# Courseware: A Web-Based Academic Resource Platform for University Students

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

Academic continuity is a persistent challenge in higher education environments. Students frequently encounter unavoidable circumstances — such as illness, personal emergencies, or timetable conflicts — that prevent regular class attendance, resulting in critical gaps in their understanding of course content. Furthermore, even students who attend consistently often require opportunities to revisit complex or concept-intensive material outside the classroom to consolidate their learning.

General-purpose platforms such as YouTube, while broadly accessible, are not designed to align with the specific syllabi, pedagogical structure, or academic standards of individual institutions. Consequently, students relying on such resources may encounter material that lacks the necessary depth, contextual accuracy, or curricular relevance required for academic success.

This platform was developed to address these limitations by providing a structured, institution-aligned academic support system. It enables students to revisit recorded lecture videos, consult course descriptions and learning outcomes, and access supplementary study materials — including previous year examination papers and course lecture PDFs — all curated in direct accordance with their academic curriculum. By centralizing these resources within a single platform, the system promotes self-paced learning and ensures consistent academic alignment, regardless of attendance.

---

## Project Description

Courseware is a full-stack academic resource platform developed using the **MERN stack** (MongoDB, Express.js, React, Node.js), with **Tailwind CSS** and **shadcn/ui** employed for the construction of a modern, fully responsive user interface.

The system is organized into two primary functional modules:

- **Student Module** — Provides authenticated access to courses, lecture content, and downloadable academic materials.
- **Admin (Instructor) Module** — Enables instructors to manage course content, user accounts, and supplementary resource uploads through a centralized dashboard.

---

## Project Demo

A comprehensive walkthrough of the platform's features and functionality is available via the link below:

**[Watch Project Demo](https://youtu.be/nnCBeL0TI-c)**

---

## Student Module Features

### Authentication

- A unified Login and Registration page allows new users to create an account and authenticate in a streamlined workflow.

### All Courses Page

- Presents a complete listing of all available courses spanning eight semesters, organized in a structured and visually consistent layout.

### Filter Course Page

Courses can be filtered according to the following criteria:

- **Category:** Departmental or Non-departmental
- **Type:** Theoretical or Sessional
- **Year-Semester:** Ranging from 1st Year – 1st Semester through 4th Year – 2nd Semester

A "No Course Found" message is rendered when no course satisfies the active filter conditions.

### Course Details Page

Each course page presents the following structured information:

- Course Description
- Course Learning Outcomes
- A complete listing of associated lectures

### Lecture Playback

- Lecture videos are delivered via streaming from **Cloudinary**, with corresponding video identifiers retrieved from **MongoDB** to ensure efficient and reliable media delivery.

### Additional Learning Resources

Two dedicated resource sections are accessible through the main navigation header:

- **Previous Year Questions:** Allows students to browse and view archived examination papers in PDF format.
- **Course Materials:** Provides access to downloadable lecture slides, notes, and supplementary academic documents.

---

## Admin (Instructor) Module Features

### User Management

- Presents a structured table of all registered users, displaying names and associated email addresses.
- Administrators are authorized to remove user accounts as required.

### Course Management

- Allows administrators to view, modify, or permanently remove existing courses from the platform.
- A **Create New Course** action initiates a structured, three-step course creation workflow.

#### Course Creation Workflow (3-Step Form)

**Step 1 — Course Curriculum**

- Supports bulk upload, replacement, and deletion of lecture video files.
- Videos are stored on **Cloudinary**, with their corresponding public identifiers persisted in **MongoDB**.

**Step 2 — Course Landing Page**

- Captures all essential course metadata, including:
  - Course Number (e.g., CSE 3200)
  - Title, Credit Hours, Subtitle, Description, Learning Outcomes, and Welcome Message
  - Classification fields: Category, Type, and Year-Semester

**Step 3 — Course Settings**

- Facilitates the upload of a course thumbnail image, which is stored on Cloudinary and referenced within the MongoDB document.

> **Note:** Submission of a new course requires all fields across all three steps to be fully completed.

---

### PDF Upload for Additional Resources

The administrator dashboard provides two dedicated resource management sections:

- **Course Materials**
- **Previous Year Questions**

Each section provides a self-contained management interface through which instructors can:

- Upload PDF documents via **Multer**, with files persisted to local server storage
- Review all uploaded files in a structured tabular view
- Remove individual files when they are no longer required

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
  <img src="https://github.com/user-attachments/assets/d6b6a089-a4be-492a-91bb-37e540321a8b" alt="Admin Dashboard" width="700" style="border:2px solid #000000; border-radius:8px; padding:6px; background:white; display:inline-block;" />
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
