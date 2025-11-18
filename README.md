# 🎓 Student Certificate Eligibility Automation using n8n


https://github.com/user-attachments/assets/0b9c894a-2373-430b-a03e-8ed1dd8d3f04


This project automates the process of determining student certificate eligibility (Gold, Silver, Bronze, or Not Eligible) based on marks and activity data submitted by students through Google Forms — using **n8n**, **Google Sheets**, and **Gmail** integration.

---

## 📋 Project Overview

The workflow is designed to make student evaluation and communication fully automated.  
It consists of **two main workflows**:

### 🔹 Workflow 1: Google Form Distribution
- Starts with a **Google Sheets Trigger**.
- Automatically sends a **Google Form link** to students via the **Gmail Node**.
- Students use this form to submit their **marks, quiz scores, and project details**.

### 🔹 Workflow 2: Eligibility Evaluation & Notification
- Begins with another **Google Sheets Trigger** connected to the form responses sheet.
- Uses **three IF Nodes (Gold, Silver, Bronze)** to evaluate the student’s marks and project status.
- Each IF Node applies specific conditions to determine:
  - 🥇 **Gold Certificate**
  - 🥈 **Silver Certificate**
  - 🥉 **Bronze Certificate**
  - ❌ **Not Eligible**

- Based on the result, the corresponding **Gmail Node** automatically sends an eligibility email to the student.

---

## 🧠 Eligibility Criteria

### 🥇 **Gold Certificate**
- Monthly Assessment Marks **> 80**  
- Total Tasks = **10**  
- Total Assignments = **10**  
- Quiz Marks **> 80**  
- Project Presentation = **Yes**

### 🥈 **Silver Certificate**
- Monthly Assessment Marks **between 60 and 80**  
- Total Tasks = **10**  
- Total Assignments = **10**  
- Quiz Marks **between 60 and 80**  
- Project Presentation = **Yes**

### 🥉 **Bronze Certificate**
- Monthly Assessment Marks **between 40 and 60**  
- Total Tasks = **10**  
- Total Assignments = **10**  
- Quiz Marks **between 40 and 60**  
- Project Presentation = **Yes**

### ❌ **Not Eligible**
- Does not meet any of the above criteria.

---

## ⚙️ Tech Stack

- **n8n** – Workflow automation platform  
- **Google Sheets** – For data input and storage  
- **Google Forms** – For student responses  
- **Gmail Node** – For automated notifications  

---

## 🧩 Workflow Logic
<img width="536" height="301" alt="image" src="https://github.com/user-attachments/assets/a22a08a8-e087-4d1d-b8fa-db0e0ead2ed5" />


---

📁 Workflow JSON File
You can find the exported n8n workflow JSON here: https://github.com/shubham132004/Certificate-Eligibility-Generation-using-N8N/tree/main/JSON%20FILE

---
## 💡 Key Features

-  Fully automated eligibility evaluation  
-  Dynamic and personalized email notifications  
-  Real-time integration with Google Sheets and Gmail  
-  Zero manual effort required  
-  Transparent and scalable system for academic certification  

---

## 🚀 How to Use

1. Clone or import this workflow into **n8n**.  
2. Connect your **Google Sheets**, **Gmail**, and **Google Forms** credentials.  
3. Update the Google Sheet and Form links within your workflow nodes.  
4. Set eligibility conditions in the **IF Nodes** based on your grading rules.  
5. Execute the workflow and monitor email delivery automatically.

---

## 📸 Workflow Preview

### Workflow Overview
<img width="528" height="294" alt="image" src="https://github.com/user-attachments/assets/8e8e562b-9875-4a06-8f13-531b27a6ce90" />


### Eligibility Logic (IF Node Conditions)
<img width="784" height="155" alt="image" src="https://github.com/user-attachments/assets/c891d824-914e-47db-83b3-7cfd66b88407" />


---

## 🧠 Impact

This automation reduces manual workload in checking eligibility, ensures accurate results, and speeds up communication with students regarding their certification levels.

---

## 👨‍💻 Author

**Shubham Parmar**  
💼 [GitHub Profile](https://github.com/shubham132004)  
📧 For queries or collaborations, feel free to reach out!


