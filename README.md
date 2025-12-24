# College Placement Management System – Salesforce

## 📌 Project Overview
The College Placement Management System is a Salesforce-based application developed to manage and automate the campus placement process in educational institutions. The system centralizes student records, company details, interview schedules, and placement results, providing real-time insights through automation, reports, and dashboards.
This project demonstrates practical Salesforce Admin skills including custom objects, relationships, validation rules, flows, and analytics.

## 🎯 Objectives
- Centralize placement-related data for students and companies  
- Track interview rounds and placement outcomes  
- Automate placement status updates using Salesforce Flow  
- Generate analytical reports and dashboards  
- Reduce manual effort and improve data accuracy  

## 🛠️ Technologies Used
- **Platform:** Salesforce Lightning Experience  
- **Automation:** Salesforce Flow Builder  
- **Analytics:** Salesforce Reports & Dashboards  

## 🧩 System Architecture
The application is built using three custom Salesforce objects:

- **Student** – Stores student academic and placement details  
- **Company** – Stores recruiting company information  
- **Placement** – Manages interview scheduling and placement results  

These objects are connected using lookup relationships to support multiple interview attempts and placements.

## 📂 Custom Objects

### Student
- Student Name  
- Roll Number (Unique)  
- Department  
- CGPA  
- Email  
- Phone  
- Placement Status (Placed / Not Placed)

### Company
- Company Name  
- Industry  
- Job Role  
- Package (CTC)  
- Location  

### Placement
- Student (Lookup)  
- Company (Lookup)  
- Interview Date  
- Interview Round  
- Status (Scheduled / Selected / Rejected)

## ⚙️ Automation
Two Salesforce record-triggered flows are implemented:
1. **Auto Schedule Interview Flow**  
   - Automatically sets placement status to *Scheduled* when a placement record is created.
2. **Update Student Placement Status Flow**  
   - Automatically updates the student’s placement status to *Placed* when the placement result is marked as *Selected*.

## ✅ Validation Rules
- Interview dates cannot be set in the past to ensure data accuracy and logical scheduling.

## 📊 Reports
- Placed vs Unplaced Students (Pie Chart)  
- Company-wise Placements (Bar Chart)  
- Upcoming Interviews (Table)

## 📈 Dashboard
**College Placement Dashboard**
- Visualizes placement statistics using multiple charts in a single dashboard:
  - Pie chart for placement status
  - Bar chart for company-wise placements
  - Table for upcoming interviews

## 👨‍💻 Author
**Venkatesh Chintada**  
Salesforce Admin Project  
Domain: Placement Management
