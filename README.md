# Attendance System for LMS (Learning Management System) in Google Apps Script

![GitHub License](https://img.shields.io/github/license/touhidulislam1999/Attendance-System-for-LMS-Learning-Management-System-in-Google-Apps-Script)

## 📌 Overview
The **Attendance System for LMS** is a web-based application designed to facilitate attendance tracking for educational institutions. Built using **Google Apps Script**, this system allows teachers to log in, take attendance, and store the data securely in **Google Sheets**. The project automates attendance management, reducing manual effort and increasing efficiency.

## 🌟 Features
- 🔐 **Login System:** Secure authentication with predefined user credentials.
- 📅 **Attendance Marking:** Teachers can mark students as **Present** or **Absent**.
- 📊 **Google Sheets Integration:** Automatically logs attendance records to Google Sheets.
- 📋 **Dynamic Class Selection:** Retrieves attendance data specific to each class.
- ⚡ **Real-time Data Fetching:** Ensures up-to-date attendance records.
- 🎨 **User-Friendly Interface:** Responsive and modern UI with form validation.
- 🚀 **Automated Data Storage:** Ensures efficient attendance tracking with a scalable solution.

## 🚀 Technologies Used
- Google Apps Script
- HTML, CSS, JavaScript
- Google Sheets API
- SweetAlert2 (for enhanced user interaction)

## 📂 Project Structure
```
📦 Attendance-System-for-LMS
 ├── 📜 Code.gs                # Main script handling HTTP requests and page rendering
 ├── 📜 Input Class.gs         # Defines user input structure
 ├── 📜 User Class.gs          # User authentication and verification class
 ├── 📜 Verify User Details.gs # Function to verify login credentials
 ├── 📜 Saved User.gs          # Stores predefined user credentials
 ├── 📜 Attendance.gs          # Fetches attendance data from Google Sheets
 ├── 📜 Submit Attendance.gs   # Handles attendance submission
 ├── 📜 Login Page.html        # Frontend login interface
 ├── 📜 Attendance Sheet.html  # Attendance sheet interface for teachers
```

## 📑 Detailed Explanation of Code Components
### 1️⃣ **Authentication System**
- The `UserClass.gs` script defines a `User` class for handling user authentication.
- The `Verify_User_Details.gs` script verifies user credentials using predefined users stored in `Saved_User.gs`.
- Upon successful login, the `login` function in `Code.gs` redirects users to the attendance sheet.

### 2️⃣ **Attendance Data Management**
- `Attendance.gs` retrieves attendance records from a Google Sheet.
- `Submit Attendance.gs` handles the submission of attendance and updates the sheet dynamically.
- Each teacher has access to a specific sheet based on their credentials.

### 3️⃣ **Frontend UI & Interaction**
- `Login Page.html` provides a login interface with validation.
- `Attendance Sheet.html` dynamically loads students and enables marking attendance.
- Includes a loader and SweetAlert2 for improved user experience.


### Step 2: Open Google Apps Script
1. Go to [Google Apps Script](https://script.google.com/)
2. Create a new project.
3. Copy and paste the files from this repository into the Apps Script editor.

### Step 3: Deploy as a Web App
1. Click **Deploy** > **New Deployment**.
2. Select **Web App** as the type.
3. Set **Execute as** to `Me`.
4. Set **Who has access** to `Anyone`.
5. Click **Deploy** and authorize permissions.
6. Copy the web app URL and share it with users.

## 🎥 Demo
![Login Page](https://github.com/user-attachments/assets/077c839e-1372-47ed-9834-8ff2ab482acc)
![Loggin In](https://github.com/user-attachments/assets/94610a85-40f5-43e6-b981-a5a0c34c270c)
![If Invalid](https://github.com/user-attachments/assets/621e81f1-f523-490e-92dc-89aa0865d52c)
![Attendance Page 1](https://github.com/user-attachments/assets/1b9294c0-11e5-49d9-b6db-81dc7dd608a6)
![Attendance Page 2](https://github.com/user-attachments/assets/b25ed63b-8c06-4ea2-9bad-9881e1f63515)
![Giving Attendance](https://github.com/user-attachments/assets/99ddea08-049b-4b6e-89b3-18570ccf47b9)
![image](https://github.com/user-attachments/assets/bffc0a71-da24-493b-8f6a-d816d679dc43)
![Submitting](https://github.com/user-attachments/assets/16b68f89-b8de-48ad-b0a8-3ccfdca27760)
![Submitted](https://github.com/user-attachments/assets/7b909551-40a3-4892-bdc4-ac978f4e315e)


![Sheet Before](https://github.com/user-attachments/assets/5177c4a0-61d8-49c2-a78b-cc8c61a0e23c)
![Sheet After](https://github.com/user-attachments/assets/95c3caf8-bc0a-4326-b6dd-fcc09ede8cd6)


## 📝 Usage Instructions
1. Open the **deployed web app**.
2. Enter valid login credentials (refer to `Saved Users.gs`).
3. Select a date and mark attendance for each student.
4. Click **Submit** to save the records.
5. Logout securely when done.

## 🔐 Security Considerations
- Only predefined users can access the attendance system.
- Uses Google Apps Script's `PropertiesService` for session management.
- Implements data validation before submission to prevent incorrect entries.

## 🔧 Setup & Installation
### Step 1: Clone the Repository
```bash
 git clone https://github.com/touhidulislam1999/Attendance-System-for-LMS-Learning-Management-System-in-Google-Apps-Script.git
```
### 📢 **Star ⭐ this repository if you found it useful!**

