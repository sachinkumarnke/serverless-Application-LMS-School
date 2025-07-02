# 📚 Serverless Student Data Management Application – AWS Project

This project demonstrates a **fully serverless web application** built using core AWS services to **collect and display student data**. It is designed to be scalable, cost-efficient, and low maintenance by leveraging **Amazon S3**, **API Gateway**, **AWS Lambda**, and **DynamoDB**.

---

## 📌 Features

- 🚀 Fully serverless architecture
- 📝 Student data submission through a web form
- 📊 Real-time data display using DynamoDB
- 🌐 Static frontend hosted on Amazon S3
- 🔐 IAM-based secure access control
- 🌍 CORS-enabled REST API with API Gateway

---

## 🛠️ Tech Stack / AWS Services Used

| AWS Service     | Role                                                |
|----------------|-----------------------------------------------------|
| **Amazon S3**   | Static website hosting (HTML, CSS, JS)              |
| **AWS Lambda**  | Backend logic to handle data storage/retrieval      |
| **API Gateway** | REST API for frontend to backend communication      |
| **DynamoDB**    | Serverless NoSQL database for student records       |
| **IAM**         | Access control and permission management            |

---

![Screenshot 2025-07-01 224401](https://github.com/user-attachments/assets/1e0f95eb-c9a3-48cf-8643-f773fd3ea763)

---

| Description                             | Screenshot |
|----------------------------------------|------------|
| 🔹 S3 Bucket Static Website Setup       |
![Screenshot 2025-07-02 105442](https://github.com/user-attachments/assets/5de3b838-061e-442e-a4c1-dabd7b62f1c8)

| 🔹 Lambda Function (Insert & Retrieve)  
![Screenshot 2025-07-01 231100](https://github.com/user-attachments/assets/d759fc2d-0baf-45f7-8423-4a3b56e43208)

| 🔹 API Gateway Integration              
![Screenshot 2025-07-01 232202](https://github.com/user-attachments/assets/61b4099e-84f9-4921-858b-c076ea14217c)

| 🔹 DynamoDB Table     
![Screenshot 2025-07-01 230126](https://github.com/user-attachments/assets/41537408-455c-4676-91c8-69e6ca81f95a)
                
| 🔹 Working Web App UI               
![Screenshot 2025-07-02 110218](https://github.com/user-attachments/assets/26c5514f-7fd5-4b45-b496-700b5d81279e)

> ⚠️ Place all your screenshots inside a [Screenshot 2025-07-02 110314](https://github.com/user-attachments/assets/50abf725-6623-4bf5-915f-be88b9f2c158)
> ![Screenshot 2025-07-02 110528](https://github.com/user-attachments/assets/c9926c8e-9c70-42f0-a2f4-8c642d4765bc)
![Screenshot 2025-07-02 110552](https://github.com/user-attachments/assets/c3ae274d-4e17-4d09-828a-ddb8412047df)

 folder in your GitHub repo and name them accordingly.

---

## 📦 How to Deploy

1. **Clone the Repo**  
   ```bash
   https://github.com/sachinkumarnke/serverless-Application-LMS-School.git


**2.** Upload Frontend to S3

Enable static website hosting

Set bucket policy to public

Upload index.html, script.js, style.css

**3.**Create DynamoDB Table

Table Name: Students

Primary Key: student_id (String)

**4.**Create Lambda Functions

add_student: Handle POST request

get_students: Handle GET request

Attach IAM roles with DynamoDB access

**5.**Create API Gateway

Configure POST /student → add_student Lambda

Configure GET /students → get_students Lambda

Enable CORS

**6.**Test the Application

Open S3 website link

Add a student and see it reflected in the table


