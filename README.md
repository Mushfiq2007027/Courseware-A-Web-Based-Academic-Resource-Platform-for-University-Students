# Courseware: A Web-Based Academic Resource Platform for University Student

---

## Table of Contents

- [Motivation](#motivation)
- [Project Description](#project-description)
- [Project Demo](#project-demo)
- [Student Module Features](#student-module-features)
- [Admin (Instructor) Module Features](#admin-instructor-module-features)
- [Screenshots](#screenshots)

---

## Motivation

In academic settings, students often face challenges in keeping up with classroom learning due to unavoidable circumstances such as illness, emergencies, or scheduling conflicts. As a result, they may miss important lectures, which directly impacts their understanding of course content. Additionally, in complex or concept-heavy subjects, students often struggle to retain everything taught in class and find themselves needing to revisit topics at a later time.

While platforms like YouTube and other online resources offer some support, they are not always aligned with the specific course structure, syllabus, and academic expectations of an institution. These general-purpose resources may lack the depth, accuracy, or contextual relevance required for academic success.

To bridge this gap and establish a more structured, syllabus-oriented academic support system, this dedicated academic courseware platform has been developed. The system allows students to revisit lecture videos, access course descriptions, review learning outcomes, and download additional study materials — including **previous year questions** and **course lecture PDFs** — all aligned with their specific curriculum.

By providing consistent and centralized access to academic materials, the platform helps students learn at their own pace and ensures they remain aligned with classroom teaching, even when absent.

---

## Project Description

This is a **full-stack academic courseware system** built using the **MERN stack** (MongoDB, Express.js, React, Node.js), along with **Tailwind CSS** and **shadcn/ui** for modern, responsive UI components.

The system consists of two major modules:

- **Student Module**
- **Admin (Instructor) Module**

---

## Project Demo

A full walkthrough of the platform is available in the video linked below:

**[Watch Project Demo](https://youtu.be/nnCBeL0TI-c)**

---

## Student Module Features

### Authentication

- Combined Login and Signup page where new users can register and subsequently log in.

### All Courses Page

- Displays all available courses across eight semesters in a clean, organized layout.

### Filter Course Page

Students can filter courses based on the following criteria:

- **Category:** Departmental or Non-departmental
- **Type:** Theoretical or Sessional
- **Year-Semester:** From 1st Year – 1st Semester to 4th Year – 2nd Semester

A "No Course Found" message is displayed if no course matches the selected criteria.

### Course Details Page

Each course detail page displays the following:

- Course Description
- Course Outcomes
- List of available Lectures

### Lecture Playback

- Students can watch lecture videos streamed from **Cloudinary**, using video IDs stored in **MongoDB**.

### Additional Learning Resources

Two dedicated resource sections are accessible via header navigation buttons:

- **Previous Year Questions:** Browse and view past exam papers in PDF format.
- **Course Materials:** Access and download lecture slides, notes, and other PDFs.

---

## Admin (Instructor) Module Features

### User Management

- Displays a table of all registered users with their names and email addresses.
- Administrators can delete user accounts if necessary.

### Course Management

- View, edit, or delete existing courses.
- A **Create New Course** button initiates a guided 3-step course creation workflow.

#### Course Creation Workflow (3-Step Form)

**Step 1 — Course Curriculum Page**
- Bulk upload, delete, or replace lecture videos.
- Videos are uploaded to **Cloudinary**, with public IDs saved in **MongoDB**.

**Step 2 — Course Landing Page**
- Enter course metadata including:
  - Course Number (e.g., CSE 3200)
  - Title, Credit, Subtitle, Description, Outcomes, and Welcome Message
  - Category, Type, and Year-Semester selection

**Step 3 — Course Settings Page**
- Upload a course thumbnail image, stored in Cloudinary and linked via MongoDB.

> **Note:** All fields must be completed before a new course can be submitted.

---

### PDF Upload for Additional Resources

Two extra dashboard buttons are available to instructors:

- **Course Materials**
- **Previous Year Questions**

Clicking either button redirects to a dedicated management page where instructors can:

- Upload PDFs via **Multer** (stored locally on the server)
- View uploaded PDFs in a structured table
- Delete PDFs when no longer needed

---

## Screenshots

**Screenshot 1: Register Page**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/c078406f-2b39-47c9-8bf6-37326e2f59fa" alt="Register Page" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 2: Home Page**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/e512a468-ade8-42d1-9c8f-60935fe52f41" alt="Home Page" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 3: Course Filter Page**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/02c9ce91-b776-4271-bdfb-740b05df2cf1" alt="Course Filter Page" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 4: Course Details Page**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/6de70cd3-5232-49c3-843e-fe0c77adf575" alt="Course Details Page" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 5: Pre-Requisite Dialog Box**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/fd7bf60e-72ac-4d9b-be66-310a5f502078" alt="Pre-Requisite Dialog Box" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 6: Play Lecture Video**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/d66eb934-b90d-490c-bda2-c3392c80a56b" alt="Play Lecture Video" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 7: View Previous Year Questions**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/1286da33-5fae-4c55-8ea8-240241279ee4" alt="View Previous Year Questions" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 8: View Course Materials**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/556cfbad-5605-4bd0-aefb-4941156e44d8" alt="View Course Materials" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 9: Admin Dashboard**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/d6b6a089-a4be-492a1-91bb-37e540321a8b" alt="Admin Dashboard" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 10: Course Listing Page**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/47331c25-fd02-4e4e-b269-697a3094ba5a" alt="Course Listing Page" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 11: Course Curriculum Page**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/d9101943-096f-4ff3-9560-395b60ec3721" alt="Course Curriculum Page" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 12: Course Landing Page**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/2732d4c3-c3e8-47d8-93c8-429db4110b49" alt="Course Landing Page" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 13: Course Image Page**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/9922cb14-2f20-4b9c-bc43-a0f4165fc1e9" alt="Course Image Page" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 14: Upload Previous Year Question PDFs**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/54b2033a-001f-4ce4-9910-df2c9a2fc864" alt="Upload Previous Year Question PDFs" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>

---

**Screenshot 15: Upload Course Material PDFs**

<div style="text-align:center; margin-bottom: 40px;">
  <img src="https://github.com/user-attachments/assets/6985cc8c-fd80-4455-b866-555da0e9a155" alt="Upload Course Material PDFs" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
</div>
