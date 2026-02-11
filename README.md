
# Introduction to Databases Project - E-Learner 

---

📁 Project name: **E-Learner**  
👥 Members: 
- **Samuele Maltauro [23928]** 
- **Kevin Joachin Trolese [23985]** 

---
## ✨ Preface    
The goal of the project is to create and implement a database 
for an **E-Learning** platform that manages online courses; lecturers are allowed 
to publish resources and materials; students can enroll in a course, attend online lectures,
and obtain certificates, after a given course is properly finished. For a course to be considered finished, students must pass all modules, and their relative exams. 

## 🔍 Overview 
The following paragraphs aim to provide an overview on the overall structure of the project, providing an insight on some decisions in relation to the ER schema.

### 👤 Users & Roles 
A `User` is an individual that uses the application, that can be either:
- a `Student`, or
- a `Professor`

such an individual has an `email` and a `password` that identifies them. 
A `User`, regardless of the type, can provide feedback to the developers. 

### 📚🛠️ Courses & Structure 
Each `Course` belongs to a `Category`, and it is composed of 1 or more `Modules`.   
Each `Module` contains various `Lectures`, and each `Lecture` may contain one or more `Resources`, may that be:
- `Videos`
- `Audios`
- `Documents`

### 📝 Enrollment & Interaction 
A `Student` can enroll in a `Course` and submit assignments if it is required.

### ✅ Evaluation
Each `Module` has its relative `Exam`. To pass a `Course`, every `Exam` in each `Module`
must be evaluated positively. At the end, the `Student` will also earn a `Certificate`,
that certifies his/her knowledge.