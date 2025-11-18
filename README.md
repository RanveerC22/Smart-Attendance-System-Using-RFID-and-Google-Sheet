# Smart Attendance System Using RFID and Google Sheet

## Intro
- This project records student attendance using RFID technology.
- When a student scans their RFID card, the attendance is automatically stored in a Google Sheet.
- The system uses NodeMCU to read RFID data and send it to Google Sheets.

## Objective
- To simplify the attendance process for teachers.
- To reduce manual work and avoid human errors.
- To create a fast, contactless, and automated attendance system.

## Process
- The project works in **3 stages**:

### 1. Reading RFID Data
- NodeMCU is connected with an RFID reader.
- When a student taps their RFID card, the device reads the unique ID.
- The student details are matched with the RFID ID.

### 2. Sending Data to Google Sheet
- NodeMCU sends the scanned RFID data to a Google Apps Script URL.
- The URL acts as an API endpoint.
- The data is pushed to the Google Sheet in real-time.

### 3. Google Sheet Script
- Google Apps Script receives the data from NodeMCU.
- The script identifies the student and marks attendance with the current date and time.
- The sheet automatically updates whenever a new scan is received.

## Features
- Contactless attendance using RFID.
- Real-time data entry into Google Sheets.
- Easy for teachers to monitor attendance.
- Reduces manual errors.
- Low-cost and simple hardware setup.

## Hardware Used
- NodeMCU ESP8266  
- RFID Reader (RC522)  
- RFID Cards/Tags  
- Jumper Wires  
- Power Source  

## Software/Tools Used
- Arduino IDE  
- Google Sheets  
- Google Apps Script  
- NodeMCU Libraries  

## How to Run
- Flash the NodeMCU code using Arduino IDE.
- Configure Wi-Fi credentials in the code.
- Deploy the Google Apps Script and also generate the sheet token to get the Web App URL.
- Update the URL in the NodeMCU code.
- Scan RFID cards to record attendance.
