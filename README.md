# Generate Yearly Reports - ACME System Automation

This repository contains an RPA project developed using UiPath to automate the process of generating and managing yearly reports for the ACME System. The automation logs into ACME System 1, reads work items, extracts relevant data, downloads reports, and uploads the reports, followed by updating the work items with the upload ID.

## 📖 Project Overview

This project automates the following steps:

1. **Login to ACME System 1**  
   - Uses credentials securely stored in UiPath Orchestrator Assets to log in.

2. **Navigate to Work Items**  
   - The robot navigates to the "Work Items" page after logging in.

3. **Read and Extract Data**  
   - Extracts key data from work items:
     - Vendor Tax ID

4. **Navigate to Download Page**  
   - Based on the extracted data, the robot navigates to the report download page.

5. **Download Reports**  
   - Downloads the reports related to the extracted data.

6. **Collect and Upload Reports**  
   - Gathers all downloaded reports and uploads them, generating an **Upload ID** for each upload.

7. **Update Work Items**  
   - Updates each work item in ACME System 1 with the corresponding upload ID.

8. **Mark Items as Completed**  
   - Marks the work item as completed once the upload is successful.

## ✨ Features

- **Automated Data Extraction:** Reads and extracts all necessary data from the work items.
- **Automated Report Download:** Automates the process of navigating to the download page and downloading reports.
- **Report Upload and ID Generation:** Uploads reports and generates an upload ID for each.
- **Work Item Update:** Automatically updates work items with the upload ID and marks them as completed.
- **Secure Login:** Uses UiPath Orchestrator Assets for secure login management.

## 🛠️ Tech Stack

- **RPA Tool:** UiPath
- **Security:** Credentials stored in UiPath Orchestrator Assets
- **File Handling:** Downloads and uploads files automatically
