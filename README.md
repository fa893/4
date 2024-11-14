<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>قائمة مشاريع الطاقة المتجددة في الأردن</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #e9ecef;
        }
        header {
            background-color: #004b87;
            color: white;
            padding: 20px;
            text-align: center;
        }
        header img {
            width: 100px;
            margin-bottom: 10px;
        }
        h1 {
            margin: 0;
            font-size: 24px;
        }
        .container {
            max-width: 90%; /* تغيير الحد الأقصى للعرض ليكون مناسبًا للهاتف */
            margin: 20px auto;
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
            box-sizing: border-box;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }
        table, th, td {
            border: 1px solid #ddd;
        }
        th, td {
            padding: 12px;
            text-align: left;
        }
        th {
            background-color: #007bff;
            color: white;
        }
        td {
            background-color: #ffffff;
        }
        label, select {
            display: block;
            margin: 10px 0;
            width: 100%;
            box-sizing: border-box;
        }
        button {
            background-color: #28a745;
            color: white;
            padding: 10px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            margin-top: 10px;
            width: 100%; /* جعل الزر يأخذ عرض كامل */
        }
        button:hover {
            background-color: #218838;
        }
        /* استجابة للهواتف */
        @media (max-width: 600px) {
            h1 {
                font-size: 20px;
            }
            th, td {
                padding: 8px;
                font-size: 14px;
            }
            button {
                font-size: 16px; /* حجم أكبر للزر على الهواتف */
            }
        }
    </style>
</head>
<body>
    <header>
        <img src="https://assets.onecompiler.app/42r523uca/42vf4yhs4/JO.png" alt="شعار الأردن">
        <h1>قائمة مشاريع الطاقة المتجددة في الأردن</h1>
        <button onclick="toggleLanguage()">Change Language</button> <!-- زر تغيير اللغة -->
    </header>
    
    <div class="container">
        <label id="locationLabel" for="locationFilter">اختر الموقع:</label>
        <select id="locationFilter" onchange="filterProjects()">
            <option value="">اختر المحافظة</option>
            <option value="Tafileh">الطفيلة</option>
            <option value="Mafraq">المفرق</option>
            <option value="Maan">معان</option>
            <option value="Aqaba">العقبة</option>
            <option value="Zarqaa">الزرقاء</option>
            <option value="Amman">عمان</option>
        </select>

        <table id="projectsTable">
            <thead>
                <tr>
                    <th id="nameColumn">اسم المشروع</th>
                    <th id="statusColumn">حالة المشروع</th>
                    <th id="locationColumn">الموقع</th>
                    <th id="ownerColumn">اسم المالك</th>
                    <th id="sizeColumn">حجم المشروع (MWAC)</th>
                    <th id="contactColumn">جهة الاتصال</th>
                </tr>
            </thead>
            <tbody>
                <!-- Tafileh Projects -->
                <tr data-location="Tafileh">
                    <td>Jordan Wind Farm</td>
                    <td>Operational since September 2015</td>
                    <td>الطفيلة</td>
                    <td>JWPC</td>
                    <td>117</td>
                    <td><a href="mailto:mjallad@jordanwind.com">mjallad@jordanwind.com</a></td>
                </tr>
                <!-- More rows here -->
            </tbody>
        </table>
    </div>

    <script>
        let isArabic = true; // لتحديد اللغة الحالية

        function toggleLanguage() {
            isArabic = !isArabic;
            if (isArabic) {
                document.documentElement.lang = 'ar';
                document.body.style.direction = 'rtl';
                document.getElementById('locationLabel').textContent = 'اختر الموقع:';
                document.getElementById('nameColumn').textContent = 'اسم المشروع';
                document.getElementById('statusColumn').textContent = 'حالة المشروع';
                document.getElementById('locationColumn').textContent = 'الموقع';
                document.getElementById('ownerColumn').textContent = 'اسم المالك';
                document.getElementById('sizeColumn').textContent = 'حجم المشروع (MWAC)';
                document.getElementById('contactColumn').textContent = 'جهة الاتصال';
            } else {
                document.documentElement.lang = 'en';
                document.body.style.direction = 'ltr';
                document.getElementById('locationLabel').textContent = 'Choose Location:';
                document.getElementById('nameColumn').textContent = 'Project Name';
                document.getElementById('statusColumn').textContent = 'Project Status';
                document.getElementById('locationColumn').textContent = 'Location';
                document.getElementById('ownerColumn').textContent = 'Owner Name';
                document.getElementById('sizeColumn').textContent = 'Project Size (MWAC)';
                document.getElementById('contactColumn').textContent = 'Contact';
            }
        }

        function filterProjects() {
            const locationFilter = document.getElementById('locationFilter').value;
            const tableRows = document.querySelectorAll('#projectsTable tbody tr');
            const projectsTable = document.getElementById('projectsTable');

            if (locationFilter) {
                projectsTable.style.display = 'table'; // Show the table
                tableRows.forEach(row => {
                    const location = row.getAttribute('data-location');
                    row.style.display = location === locationFilter ? '' : 'none';
                });
            } else {
                projectsTable.style.display = 'none'; // Hide the table if no location is selected
            }
        }
    </script>
</body>
</html>
