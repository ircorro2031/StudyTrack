## StudyTrack: A student academic peformance and management system

## Project Overview

StudyTrack is a planned application made to help students organize their academic records, monitor their performance, manage school-related responsibilities, and identify areas that need improvement.

Using JSON files for data storage, the system will provide tools for tracking grades, managing subject announcements and deadlines, recording academic mistakes, and viewing an overview of academic progress.

## Problem Statement

Students often need to manage different academic responsibilities, including monitoring grades, remembering announcements, keeping track of deadlines, and identifying topics they find difficult. When these responsibilities are handled separately, it can become challenging to stay organized and monitor academic progress.

StudyTrack aims to address this problem by providing a centralized system where students can organize their academic information and access useful summaries of their performance and responsibilities.

## Project Objectives

1. To develop an application that allows students to organize and manage their academic records
2. To give tools for monitoring grades, announcements, tasks, and academic weaknesses
3. To analyze stored academic data and present useful summaries that help students monitor their progress

## Main Features

StudyTrack is planned to have the following features:

1. Student Records Management – View and search student information from the provided dataset
2. Grade Tracker and Calculator – Add, view, update, and delete academic grade records, calculate subject averages, and determine overall academic averages
3. Announcement Manager – Store, view, update, and delete announcements organized by subject
4. Task and Deadline Manager – Record school tasks, assign due dates and priorities, and monitor completion status
5. Mistake and Weakness Logger – Record academic mistakes, identify difficult topics, and monitor recurring areas of difficulty
6. Academic Performance Dashboard – Present academic summaries, subject performance, task progress, and mistake statistics

## Dataset and Data Storage

The project will use the provided "students.json" dataset as its initial source of student information and academic grades.

Additional information entered through the application will be stored in separate JSON files:

- "students.json" – Initial student records and subject grades
- "academic_records.json" – Additional academic records organized by student, subject, and quarter
- "announcements.json" – Subject announcements and related information
- "tasks.json" – Academic tasks, deadlines, priorities, and completion statuses
- "mistakes.json" – Recorded academic mistakes, difficult topics, and corrections

The original dataset will be unchanged. Additional records will be stored separately to support the application's features.

## Technologies

- Programming Language: Python
- Data Storage: JSON
- Development Platform: GitHub/OnlineGDB

## Planned Repository Structure

StudyTrack/
│
├── data/
│   ├── students.json
│   ├── academic_records.json
│   ├── announcements.json
│   ├── tasks.json
│   └── mistakes.json
│
├── docs/
│   └── proposal_template.md
│
├── README.md
└── main.py

Note: Additional files and folders may be added as the project develops

## Project Status

Current Stage: PROJECT MILESTONE

Our group is still developing the project proposal, making the system's features, planning the data requirements, and preparing the initial program design. Actual implementation, testing, and improvements will follow in the next project milestones.

## Group Members

- Member 1: Emmbert Matthieu O. Cebrian
- Member 2: Iza Rafaelle T. Corro
- Member 3: Rogen Gil R. Tan
