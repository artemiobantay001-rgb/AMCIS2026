# AMCIS Biometric Attendance Analyzer

A browser-based attendance analyzer for biometric CSV/Excel exports.

## Features
- Upload `.csv`, `.xlsx`, or `.xls` biometric attendance data.
- Automatically detects Name, Date, and Time columns, with manual selection available.
- Select an attendance date or automatically use the latest date in the file.
- Choose how many **Late Comers** and **Early Birds** to display.
- Shows late comers ranked by latest arrival time and early birds ranked by earliest arrival time.
- Exports the selected results to CSV and supports printing.
- Attendance data is processed locally in the browser; it is not uploaded to a server by this application.

## Expected biometric data
The application works best with rows containing a person's name, attendance date, and arrival/check-in time. Common column names such as `Name`, `Date`, `Time`, `Employee Name`, `Check In`, and `Timestamp` are detected automatically.

## Important
The current version treats the earliest recorded time for each person on the selected date as their arrival time. A school-specific official late threshold (for example, 7:31 AM) is not hard-coded; therefore, "Late Comers" currently means the people with the latest arrival times. A configurable official start time can be added if required.

## Run
Open `index.html` in a modern browser. No server is required.
