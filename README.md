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
            background-color: #e9ecef; /* لون خلفية أكثر رسمية */
        }
        header {
            background-color: #004b87; /* لون رمزي للحكومة */
            color: white;
            padding: 20px;
            text-align: center;
        }
        header img {
            width: 100px; /* عرض الشعار */
            margin-bottom: 10px;
        }
        h1 {
            margin: 0;
            font-size: 24px;
        }
        .container {
            max-width: 900px;
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
            background-color: #007bff; /* لون مميز للعناوين */
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
            background-color: #28a745; /* لون الزر */
            color: white;
            padding: 10px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            margin-top: 10px;
        }
        button:hover {
            background-color: #218838; /* لون الزر عند التمرير */
        }
        @media (max-width: 600px) {
            h1 {
                font-size: 20px; /* حجم خط أصغر على الهواتف */
            }
            th, td {
                padding: 8px;
                font-size: 14px; /* حجم خط أصغر على الهواتف */
            }
        }
    </style>
</head>
<body>
    <header>
        <img src="https://assets.onecompiler.app/42r523uca/42vf4yhs4/JO.png" alt="شعار الأردن">
        <h1>قائمة مشاريع الطاقة المتجددة في الأردن</h1>
    </header>
    
    <div class="container">
        <label for="locationFilter">اختر الموقع:</label>
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
                    <th>اسم المشروع</th>
                    <th>حالة المشروع</th>
                    <th>الموقع</th>
                    <th>اسم المالك</th>
                    <th>حجم المشروع (MWAC)</th>
                    <th>جهة الاتصال</th>
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
                    <td><a href="mailto: mjallad@jordanwind.com">mjallad@jordanwind.com</a></td>
                </tr>
                <tr data-location="Tafileh">
                    <td>Wind energy project - Mass</td>
                    <td>Operational since July 2020</td>
                    <td>الطفيلة</td>
                    <td>Mass Energy</td>
                    <td>100</td>
                    <td><a href="mailto: khaled.abualshaikh@massgroupholding.com">khaled.abualshaikh@massgroupholding.com</a></td>
                </tr>
                <!-- Mafraq Projects -->
                <tr data-location="Mafraq">
                    <td>Al-Badiya Philadelphia</td>
                    <td>Operational since October 2015</td>
                    <td>المفرق</td>
                    <td>Philadelphia Solar</td>
                    <td>13</td>
                    <td><a href="mailto: a.smadi@philadelphia-solar.com">a.smadi@philadelphia-solar.com</a></td>
                </tr>
                <tr data-location="Mafraq">
                    <td>Direct Proposal/ Round 1 PV/ Jordan Solar One</td>
                    <td>Operational since September 2016</td>
                    <td>المفرق</td>
                    <td>Jordan Solar One</td>
                    <td>20</td>
                    <td><a href="mailto: Projects.jordan@outlook.com">Projects.jordan@outlook.com</a></td>
                </tr>
                <!-- Maan Projects -->
                <tr data-location="Maan">
                    <td>Direct Proposal/ Round 1 PV/ Scatec Solar</td>
                    <td>Operational since June 2016</td>
                    <td>معان</td>
                    <td>Scatec Solar</td>
                    <td>10</td>
                    <td><a href="mailto: iyad.assaf@scatecsolar.com">iyad.assaf@scatecsolar.com</a></td>
                </tr>
                <tr data-location="Maan">
                    <td>Direct Proposal/ Round 1 PV/ SunEdison Project</td>
                    <td>Operational since July 2016</td>
                    <td>معان</td>
                    <td>Adwa’a Maân</td>
                    <td>20</td>
                    <td><a href="mailto: mahmoud_alhamaideh@ctgsail.com">mahmoud_alhamaideh@ctgsail.com</a></td>
                </tr>
                <!-- Aqaba Projects -->
                <tr data-location="Aqaba">
                    <td>Direct proposals/ Round 1 PV/ Shamsuna</td>
                    <td>Operational since February 2016</td>
                    <td>العقبة</td>
                    <td>Shamsuna</td>
                    <td>10</td>
                    <td><a href="mailto: Tamerk@falconmaan.com">Tamerk@falconmaan.com</a></td>
                </tr>
                <tr data-location="Aqaba">
                    <td>Al-Qweira PV Plant - Gulf Grant</td>
                    <td>Operational since July 2018</td>
                    <td>العقبة</td>
                    <td>Government</td>
                    <td>92</td>
                    <td><a href="mailto: okasasbeh@sepco.com.jo">okasasbeh@sepco.com.jo</a></td>
                </tr>
                <!-- Zarqaa Projects -->
                <tr data-location="Zarqaa">
                    <td>Azraq Camp Solar PV Plant</td>
                    <td>Operational since April 2015</td>
                    <td>الزرقاء</td>
                    <td>Government</td>
                    <td>2</td>
                    <td><a href="mailto: smaani@sepco.com.jo">smaani@sepco.com.jo</a></td>
                </tr>
                <tr data-location="Zarqaa">
                    <td>Expansion of Azraq PV plant</td>
                    <td>Operational since February 2020</td>
                    <td>الزرقاء</td>
                    <td>Government</td>
                    <td>5</td>
                    <td><a href="mailto: smaani@sepco.com.jo">smaani@sepco.com.jo</a></td>
                </tr>
                <!-- Amman Projects -->
                <tr data-location="Amman">
                    <td>East Amman PV project</td>
                    <td>Operational since September 2019</td>
                    <td>عمان</td>
                    <td>AES/Mitsui</td>
                    <td>40</td>
                    <td><a href="mailto: khaled.othman@aes.com">khaled.othman@aes.com</a></td>
                </tr>
                <tr data-location="Amman">
                    <td>Baynona PV project</td>
                    <td>Operational since December 2020</td>
                    <td>عمان</td>
                    <td>Masdar</td>
                    <td>200</td>
                    <td><a href="mailto: malmasri@baynouna.jo">malmasri@baynouna.jo</a></td>
                </tr>
            </tbody>
        </table>
    </div>

    <script>
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
