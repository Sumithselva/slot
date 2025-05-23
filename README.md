# Ex03 Time Table
## Date:22.05.2025

## AIM
To write a html webpage page to display your slot timetable.

## ALGORITHM
### STEP 1
Create a Django-admin Interface.

### STEP 2
Create a static folder and inert HTML code.

### STEP 3
Create a simple table using ```<table>``` tag in html.

### STEP 4
Add header row using ```<th>``` tag.

### STEP 5
Add your timetable using ```<td>``` tag.

### STEP 6
Execute the program using runserver command.

## PROGRAM
```
<html>
<head>
    <title>Official Timetable</title>
    <style>
        :root {
            --primary-color: #2e7d32; /* Dark green */
            --secondary-color: #e8f5e9; /* Light green */
            --text-color: #1b1b1b;
            --bg-color: #f1f8e9;
            --border-color: #1b5e20;
            --header-bg: #388e3c;
            --header-text: white;
            --highlight-bg: #1b5e20;
            --highlight-text: white;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: var(--bg-color);
            color: var(--text-color);
            padding: 30px;
        }

        .container {
            max-width: 1000px;
            margin: auto;
            background: white;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            border: 2px solid var(--border-color);
        }

        .header {
            text-align: center;
            margin-bottom: 10px;
        }

        .header img {
            max-width: 500px;
            height: auto;
            display: block;
            margin: 0 auto;
        }

        h1 {
            font-size: 35px;
            margin-top: 10px;
            color: var(--primary-color);
            letter-spacing: 1px;
            font-weight: 600;
        }

        .info {
            text-align: center;
            font-size: 20px;
            margin-bottom: 10px;
            font-weight: 500;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 30px;
        }

        th, td {
            border: 2px solid var(--border-color);
            padding: 12px;
            text-align: center;
            font-size: 14px;
        }

        th {
            background-color: var(--header-bg);
            color: var(--header-text);
            font-weight: 600;
        }

        td.day {
            background-color: var(--highlight-bg);
            color: var(--highlight-text);
            font-weight: bold;
        }

        td.lunch {
            background-color: var(--secondary-color);
            font-weight: bold;
        }

        tr:nth-child(even) {
            background-color: var(--secondary-color);
        }

        .subject-title {
            font-size: 26px;
            text-align: center;
            font-weight: 600;
            margin-bottom: 15px;
            color: var(--primary-color);
        }

        .subject-table th {
            background-color: var(--header-bg);
            color: var(--header-text);
        }
    </style>
</head>
<body>

<div class="container">
    <div class="header">
        <img src="/static/logo.png" alt="Saveetha Logo">
        <h1>OFFICIAL TIMETABLE</h1>
    </div>

    <div class="info">
        <strong>Name:</strong> SUMITH &nbsp; | &nbsp;
        <strong>Reg No:</strong> 212224230279
    </div>

    <table>
        <thead>
            <tr>
                <th>DAY</th>
                <th>8:00 - 10:00</th>
                <th>10:00 - 12:00</th>
                <th>12:00 - 1:00</th>
                <th>1:00 - 3:00</th>
                <th>3:00 - 5:00</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td class="day">MON</td>
                <td></td>
                <td></td>
                <td class="lunch">LUNCH</td>
                <td>Data Structures</td>
                <td></td>
            </tr>
            <tr>
                <td class="day">TUES</td>
                <td>Maths</td>
                <td></td>
                <td class="lunch">LUNCH</td>
                <td></td>
                <td>Java Programming</td>
            </tr>
            <tr>
                <td class="day">WED</td>
                <td></td>
                <td>Java Programming</td>
                <td class="lunch">LUNCH</td>
                <td>Project Lab</td>
                <td>Environmental Science</td>
            </tr>
            <tr>
                <td class="day">THURS</td>
                <td>Maths</td>
                <td>Java Programming</td>
                <td class="lunch">LUNCH</td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td class="day">FRI</td>
                <td>Maths</td>
                <td></td>
                <td class="lunch">LUNCH</td>
                <td></td>
                <td>Soft Skills</td>
            </tr>
            <tr>
                <td class="day">SAT</td>
                <td></td>
                <td>Java Programming</td>
                <td class="lunch">LUNCH</td>
                <td>Environmental Science</td>
                <td>Data Structures</td>
            </tr>
        </tbody>
    </table>

    <div class="subject-title">Subject Details</div>
    <table class="subject-table">
        <thead>
            <tr>
                <th>S.No</th>
                <th>Subject Code</th>
                <th>Subject Name</th>
            </tr>
        </thead>
        <tbody>
            <tr><td>1</td><td>19CS101</td><td>Java Programming</td></tr>
            <tr><td>2</td><td>19CS102</td><td>Data Structures</td></tr>
            <tr><td>3</td><td>19MA103</td><td>Engineering Mathematics</td></tr>
            <tr><td>4</td><td>19EN104</td><td>Environmental Science</td></tr>
            <tr><td>5</td><td>19PD105</td><td>Soft Skills</td></tr>
        </tbody>
    </table>

    <center>
        <footer>
            @2025 Official TimeTable. All rights reserved.
        </footer>
    </center>

</div>

</body>
</html>

```

## OUTPUT
![alt text](<Screenshot (27).png>)

## RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
