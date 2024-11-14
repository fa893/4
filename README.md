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
        h1 {
            margin: 0;
            font-size: 24px;
        }
        .container {
            max-width: 90%;
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
            width: 100%;
        }
        button:hover {
            background-color: #218838;
        }
        @media (max-width: 600px) {
            h1 {
                font-size: 20px;
            }
            th, td {
                padding: 8px;
                font-size: 14px;
            }
            button {
                font-size: 16px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>قائمة مشاريع الطاقة المتجددة في الأردن</h1>
    </header>
    
    <div class="container">
        <label for="locationFilter">اختر الموقع (Select Location):</label>
        <select id="locationFilter" onchange="filterProjects()">
            <option value="">اختر المحافظة (Select Governorate)</option>
            <option value="Tafileh">الطفيلة (Tafileh)</option>
            <option value="Mafraq">المفرق (Mafraq)</option>
            <option value="Maan">معان (Maan)</option>
            <option value="Aqaba">العقبة (Aqaba)</option>
            <option value="Zarqaa">الزرقاء (Zarqaa)</option>
            <option value="Amman">عمان (Amman)</option>
        </select>

        <table id="projectsTable">
            <thead>
                <tr>
                    <th>اسم المشروع (Project Name)</th>
                    <th>حالة المشروع (Project Status)</th>
                    <th>الموقع (Location)</th>
                    <th>اسم المالك (Owner)</th>
                    <th>حجم المشروع (MWAC)</th>
                    <th>جهة الاتصال (Contact)</th>
                </tr>
            </thead>
            <tbody>
                <!-- Tafileh Projects -->
                <tr data-location="Tafileh">
                    <td>Jordan Wind Farm</td>
                    <td>Operational since September 2015</td>
                    <td>الطفيلة (Tafileh)</td>
                    <td>JWPC</td>
                    <td>117</td>
                    <td><a href="mailto:mjallad@jordanwind.com">mjallad@jordanwind.com</a></td>
                </tr>
                <tr data-location="Tafileh">
                    <td>Wind energy project - Mass</td>
                    <td>Operational since July 2020</td>
                    <td>الطفيلة (Tafileh)</td>
                    <td>Mass Energy</td>
                    <td>100</td>
                    <td><a href="mailto:khaled.abualshaikh@massgroupholding.com">khaled.abualshaikh@massgroupholding.com</a></td>
                </tr>
                <!-- Mafraq Projects -->
                <tr data-location="Mafraq">
                    <td>Al-Badiya Philadelphia</td>
                    <td>Operational since October 2015</td>
                    <td>المفرق (Mafraq)</td>
                    <td>Philadelphia Solar</td>
                    <td>13</td>
                    <td><a href="mailto:a.smadi@philadelphia-solar.com">a.smadi@philadelphia-solar.com</a></td>
                </tr>
                <tr data-location="Mafraq">
                    <td>Direct Proposal/ Round 1 PV/ Jordan Solar One</td>
                    <td>Operational since September 2016</td>
                    <td>المفرق (Mafraq)</td>
                    <td>Jordan Solar One</td>
                    <td>20</td>
                    <td><a href="mailto:Projects.jordan@outlook.com">Projects.jordan@outlook.com</a></td>
                </tr>
                <!-- Maan Projects -->
                <tr data-location="Maan">
                    <td>Direct Proposal/ Round 1 PV/ Scatec Solar</td>
                    <td>Operational since June 2016</td>
                    <td>معان (Maan)</td>
                    <td>Scatec Solar</td>
                    <td>10</td>
                    <td><a href="mailto:iyad.assaf@scatecsolar.com">iyad.assaf@scatecsolar.com</a></td>
                </tr>
                <tr data-location="Maan">
                    <td>Direct Proposal/ Round 1 PV/ SunEdison Project</td>
                    <td>Operational since July 2016</td>
                    <td>معان (Maan)</td>
                    <td>Adwa’a Maân</td>
                    <td>20</td>
                    <td><a href="mailto:mahmoud_alhamaideh@ctgsail.com">mahmoud_alhamaideh@ctgsail.com</a></td>
                </tr>
                <!-- Aqaba Projects -->
                <tr data-location="Aqaba">
                    <td>Direct proposals/ Round 1 PV/ Shamsuna</td>
                    <td>Operational since February 2016</td>
                    <td>العقبة (Aqaba)</td>
                    <td>Shamsuna</td>
                    <td>10</td>
                    <td><a href="mailto:Tamerk@falconmaan.com">Tamerk@falconmaan.com</a></td>
                </tr>
                <tr data-location="Aqaba">
                    <td>Al-Qweira PV Plant - Gulf Grant</td>
                    <td>Operational since July 2018</td>
                    <td>العقبة (Aqaba)</td>
                    <td>Government</td>
                    <td>92</td>
                    <td><a href="mailto:okasasbeh@sepco.com.jo">okasasbeh@sepco.com.jo</a></td>
                </tr>
                <!-- Zarqaa Projects -->
                <tr data-location="Zarqaa">
                    <td>Azraq Camp Solar PV Plant</td>
                    <td>Operational since April 2015</td>
                    <td>الزرقاء (Zarqaa)</td>
                    <td>Government</td>
                    <td>2</td>
                    <td><a href="mailto:smaani@sepco.com.jo">smaani@sepco.com.jo</a></td>
                </tr>
                <tr data-location="Zarqaa">
                    <td>Expansion of Azraq PV plant</td>
                    <td>Operational since February 2020</td>
                    <td>الزرقاء (Zarqaa)</td>
                    <td>Government</td>
                    <td>5</td>
                    <td><a href="mailto:smaani@sepco.com.jo">smaani@sepco.com.jo</a></td>
                </tr>
                <!-- Amman Projects -->
                <tr data-location="Amman">
                    <td>Direct Proposal/ Round 2 PV/ Jordanian Engineers Union</td>
                    <td>Operational since May 2016</td>
                    <td>عمان (Amman)</td>
                    <td>Jordanian Engineers Union</td>
                    <td>5</td>
                    <td><a href="mailto:saleh@geejordan.com">saleh@geejordan.com</a></td>
                </tr>
                <tr data-location="Amman">
                    <td>Jordan Solar PV Project - Al-Ayla</td>
                    <td>Operational since September 2015</td>
                    <td>عمان (Amman)</td>
                    <td>Al-Ayla</td>
                    <td>20</td>
                    <td><a href="mailto:alrube@ayla.com.jo">alrube@ayla.com.jo</a></td>
                </tr>
            </tbody>
        </table>
    </div>

    <script>
        function filterProjects() {
            var filter = document.getElementById("locationFilter").value;
            var rows = document.querySelectorAll("#projectsTable tbody tr");

            rows.forEach(row => {
                if (filter === "" || row.getAttribute("data-location") === filter) {
                    row.style.display = "";
                } else {
                    row.style.display = "none";
                }
            });
        }
    </script>
</body>
</html>
