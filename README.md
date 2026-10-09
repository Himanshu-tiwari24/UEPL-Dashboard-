# UEPL Attendance Dashboard

An interactive attendance management dashboard for **Utsah Engineering Pvt. Ltd. (UEPL)** that helps visualize employee attendance, department-wise performance, daily in/out timings, and attendance records using an Excel Performance Register.

## Overview

The UEPL Attendance Dashboard is a browser-based dashboard built with HTML, CSS, and JavaScript. It provides a centralized view of employee attendance information and allows users to upload an Excel Performance Register to update the dashboard.

## Features

- **Overview Dashboard:** KPI cards, attendance status breakdown, attendance trends, and department comparisons.
- **Department Analysis:** Department-wise attendance percentages, employee counts, present and absent days, weekly offs, half days, and MIS records.
- **Employee Attendance Register:** Search, sort, and filter employees by name, employee code, department, attendance percentage, and status.
- **Daily Attendance:** View employee attendance records, including in-time, out-time, and attendance status.
- **Attendance Calendar:** Calendar-based view of daily employee attendance.
- **Excel Upload:** Upload `.xlsx` and `.xls` Performance Register files.
- **Data Update Modes:** Replace existing dashboard data or append/merge uploaded employee records.
- **Data Quality Summary:** Identify duplicate employee IDs, missing departments, missing in/out times, MIS records, and records requiring review.
- **Upload History:** Review file names, upload timestamps, employee counts, and update modes.
- **Responsive Design:** Dark-themed interface designed to adapt to different screen sizes.

## Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Dashboard structure |
| CSS3 | Styling and responsive layout |
| JavaScript | Dashboard logic and data processing |
| Chart.js 4.4.1 | Interactive charts and visualizations |
| SheetJS (xlsx) 0.18.5 | Reading Excel files in the browser |
| GitHub Pages | Optional static website hosting |

## Project Structure

```text
UEPL-Attendance-Dashboard/
│
├── index.html
└── README.md
```

The main dashboard HTML file should be renamed to `index.html` before deploying it through GitHub Pages.

## How to Run Locally

1. Download or clone this repository.
2. Open the project folder.
3. Rename `UEPL_Attendance_Dashboard (1).html` to `index.html`.
4. Open `index.html` in Google Chrome or another modern browser.
5. Use the **Upload New Excel** button to upload the UEPL Performance Register.

An internet connection is required to load the Chart.js and SheetJS libraries from their CDNs.

## How to Upload Attendance Data

1. Open the dashboard.
2. Click **Upload New Excel**.
3. Select the monthly UEPL Performance Register in `.xlsx` or `.xls` format.
4. Review the data quality summary.
5. Select an update mode:
   - **Replace Current Data:** Replace the existing employee records with the uploaded records.
   - **Append to Existing:** Merge uploaded employee records with existing records, updating matching employee IDs and retaining employees not present in the new file.
6. Click **Apply & Update Dashboard**.
7. Review the updated dashboard, department statistics, employee records, and upload history.

**Important:** Uploading a file updates the dashboard in the current browser session. The current implementation does not persist uploaded data to a database or automatically synchronize it across different users or devices. Refreshing the page or reopening it may restore the built-in sample data.

## Deploy on GitHub Pages

1. Create a new repository on GitHub, for example, `UEPL-Attendance-Dashboard`.
2. Upload `index.html` and `README.md` to the repository's root directory.
3. Open the repository's **Settings**.
4. Select **Pages** from the sidebar.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select the `main` branch and `/ (root)` folder.
7. Click **Save**.
8. Wait for GitHub Pages to publish the website.
9. Open the URL provided in the Pages settings.

GitHub Pages can host the static dashboard, but it does not provide shared storage or a database for uploaded attendance data.

## Data Privacy

Attendance registers contain employee information. Upload only authorized company data, restrict access to the repository and dashboard as appropriate, and avoid publishing real employee records in a public repository.

## Future Improvements

- Connect the dashboard to a shared Google Sheet or database.
- Enable automatic attendance data synchronization.
- Add user authentication and role-based access.
- Export filtered attendance reports to Excel or PDF.
- Add monthly and yearly attendance comparisons.
- Deploy through an internal company portal for authorized employees.

## Disclaimer

This project is intended for internal attendance monitoring and reporting. The dashboard's accuracy depends on the uploaded Performance Register and the data parsing rules implemented in the application.

---

**Developed for:** Utsah Engineering Pvt. Ltd. (UEPL)

**Project:** UEPL Attendance Dashboard

**Category:** HR Analytics | Attendance Management | MIS Reporting
