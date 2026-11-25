## 📝 Project Title


StudyTrack: A student academic performance and management system


## 🔍 Project Description


StudyTrack is an application designed to help students organize their academic information, monitor their performance, and manage their school responsibilities in one system.


The application will provide features for managing student academic records, tracking grades, calculating academic averages, organizing announcements and deadlines, and recording mistakes to identify areas that need improvement. It will also generate an academic dashboard that presents useful summaries and statistics based on the information stored in the system.


Using the 'students.json' dataset as the initial source of student information and academic grades, StudyTrack will allow users to explore existing records and maintain additional academic information through separate JSON files. The application aims to make academic management more organized while demonstrating the practical use of Python programming, data processing, and persistent data storage.


## 🔍 Problem Statement


Students handle many different academic responsibilities, including monitoring their grades, remembering deadlines, keeping track of announcements, and identifying subjects or topics that require improvement. When these responsibilities and records are managed separately, it can become difficult to maintain an organized overview of one's academic progress.


StudyTrack aims to address this problem by providing an application where academic records and school-related responsibilities can be organized and monitored. Through its grade tracker, academic organizer, and mistake and weakness logger, students can manage their information, review their performance, and identify areas that need attention.


The project will use the given 'students.json' dataset, which has student identifiers, names, sections, and grades across different subjects. Additional information, such as quarter grades, announcements, tasks, deadlines, and recorded mistakes, will be collected and stored in separate JSON files.


By combining academic record management with basic data analysis, StudyTrack will help users gain meaningful insights into their academic performance and develop more organized study habits.


## 🎯 Project Objectives


1. To create an application that allows users to organize and manage academic records and school-related information

2. To implement Create, Read, Update, and Delete (CRUD) operations for managing grades, announcements, tasks, and academic mistake records

3. To calculate academic averages and generate meaningful summaries and comparisons based on stored student grades

4. To help users monitor academic responsibilities, recognize recurring mistakes, and identify areas that need improvement

5. To apply Python programming concepts, JSON file handling, input validation, and descriptive statistical techniques in developing a functional application


## ⚙️ Planned Features


### A. Academic Records and Grade Tracker


**1. Student Records Management**


- Display student information retrieved from the given 'students.json' dataset

- Search for students using their ID or name

- View their corresponding section and recorded subject grades


**2. Grade Tracker and Calculator**


- Add, view, update, and delete academic grade records

- Organize additional grade records according to subject and grading quarter

- Calculate subject averages and overall academic averages

- Generate an estimated GWA based on available grades, using the selected calculation method


### B. Academic Organizer


**3. Announcement Manager**


- Add and store academic announcements

- Organize announcements according to subject

- View, update, and delete stored announcements


**4. Task and Deadline Manager**


- Add assignments, projects, examinations, and other academic tasks

- Set task descriptions, subjects, priorities, and due dates

- View pending and completed tasks

- Update task details and mark tasks as completed

- Edit or delete existing tasks


### C. Academic Improvement


**5. Mistake and Weakness Logger**


- Record mistakes from quizzes, examinations, and other academic activities

- Categorize mistakes, such as conceptual misunderstandings, careless errors, and incorrect methods

- Record the subject, topic, explanation of the mistake, and correct understanding

- Review previous mistakes and identify recurring areas of difficulty


### D. Academic Dashboard


**6. Academic Performance Dashboard**


- Display an overview of the user's academic records

- Present calculated grade averages and subject performance

- Show pending and completed tasks

- Summarize recorded mistakes and frequently occurring categories

- Provide comparisons and statistics based on available information


## ⌨️ Planned Inputs and Outputs


### Inputs


StudyTrack will accept the following information from users:


**Academic Records and Grades**

- Student ID or name for searching student information

- Subject name

- Grading quarter

- Grade or academic result

- Record details for adding, updating, or deleting grades


**Announcements**

- Announcement title

- Subject or category

- Announcement description

- Date or relevant deadline, if applicable


**Tasks and Deadlines**

- Task or assignment name

- Subject

- Description

- Due date

- Priority level

- Completion status


**Mistake and Weakness Logger**

- Subject and topic

- Description of the mistake

- Mistake category

- Correct understanding or explanation


**Navigation**

- Menu selections and search terms


### Outputs


StudyTrack will display:


- Student information and recorded subject grades

- Organized academic records by student, subject, and quarter

- Calculated subject averages and estimated overall academic averages

- Stored announcements organized by subject

- Lists of pending and completed academic tasks

- Recorded mistakes categorized according to their causes

- Summaries of recurring mistakes and areas for improvement

- An academic dashboard containing relevant statistics, summaries, and comparisons

- Confirmation messages and error notifications for user actions


## 📂 Description of Data to Be Collected and Stored


StudyTrack will use JSON files to store and manage its information. The given 'students.json' dataset will serve as the initial source of student profiles and existing subject grades.


Additional information will be stored separately to preserve the original dataset.


### Planned JSON Files


| JSON File | Information Stored |

|---|---|

| 'students.json' | Student IDs, names, sections, and existing subject grades |

| 'academic_records.json' | Additional grades organized by student, subject, and quarter |

| 'announcements.json' | Announcement titles, subjects, descriptions, and dates |

| 'tasks.json' | Task names, descriptions, subjects, due dates, priorities, and statuses |

| 'mistakes.json' | Recorded mistakes, subjects, topics, categories, and corrections |


### Sample Data Structure


**Example: academic_records.json**


```json

{

  "academic_records": [

    {

      "record_id": 1,

      "student_id": 1,

      "subject": "Mathematics",

      "quarter": "Quarter 1",

      "grade": 1.75

    }

  ]

}

```


**Example: tasks.json**


```json

{

  "tasks": [

    {

      "task_id": 1,

      "title": "Mathematics Assignment",

      "subject": "Mathematics",

      "due_date": "2026-12-05",

      "priority": "High",

      "status": "Pending"

    }

  ]

}

```


**Example: mistakes.json**


```json

{

  "mistakes": [

    {

      "mistake_id": 1,

      "student_id": 1,

      "subject": "Mathematics",

      "topic": "Algebra",

      "category": "Conceptual Misunderstanding",

      "description": "Difficulty understanding the concept.",

      "correction": "Review the lesson and practice related problems."

    }

  ]

}

```


These are initial examples only. They may be changed and adjusted during the actual development.


### Data Management and Validation


The application will implement CRUD operations to allow users to create, view, update, and delete stored records.


It will also apply input validation to help ensure that:

- Required fields are not left empty

- Grade inputs are valid numerical values

- Dates follow the required format

- Selected categories and priorities are valid

- Record identifiers are unique

- Invalid menu selections are handled appropriately


The application will save changes to the corresponding JSON files so that records remain available when the program is opened again.


## 🧠 Logic Plan


### Pseudocode


```text

START


Load student records from students.json

Load academic records from academic_records.json

Load announcements from announcements.json

Load tasks from tasks.json

Load mistakes from mistakes.json


Display the StudyTrack main menu


REPEAT


    Ask the user to select a module


    IF the user selects 1:

        Display student records

        Allow the user to search for a student

        Display the selected student's academic information


    ELSE IF the user selects 2:

        Display grade tracker options

        Allow the user to add, view, update, or delete grade records

        Calculate academic averages when requested

        Save changes to academic_records.json


    ELSE IF the user selects 3:

        Display announcement management options

        Allow the user to add, view, update, or delete announcements

        Save changes to announcements.json


    ELSE IF the user selects 4:

        Display task management options

        Allow the user to add, view, update, or delete tasks

        Allow the user to update task completion status

        Save changes to tasks.json


    ELSE IF the user selects 5:

        Display mistake and weakness logger options

        Allow the user to record, view, update, or delete mistakes

        Analyze recurring mistake categories

        Save changes to mistakes.json


    ELSE IF the user selects 6:

        Calculate available academic statistics

        Summarize pending tasks and recorded mistakes

        Display the academic dashboard


    ELSE IF the user selects 7:

        Display an exit message


    ELSE:

        Display an invalid choice message


UNTIL the user chooses to exit


END

```


### Sample Wireframe


The following wireframe illustrates the proposed console interface and how users will interact with StudyTrack.


**1. Main Menu**


```text

================================================

                   STUDYTRACK

       STUDENT ACADEMIC PERFORMANCE SYSTEM

================================================


[1] Student Academic Records

[2] Grade Tracker and Calculator

[3] Announcement Manager

[4] Task and Deadline Manager

[5] Mistake and Weakness Logger

[6] Academic Performance Dashboard

[7] Exit


------------------------------------------------

Enter your choice: _

================================================

```


**2. Grade Tracker**


```text

================================================

                  GRADE TRACKER

================================================


[1] View Grade Records

[2] Add Grade Record

[3] Update Grade Record

[4] Delete Grade Record

[5] Calculate Academic Average

[6] Return to Main Menu


------------------------------------------------

Enter your choice: _

================================================

```


**3. Academic Performance Dashboard**


```text

================================================

             ACADEMIC DASHBOARD

================================================


STUDENT: Sample Student

SECTION: Sample Section


-----------------------------------------------

ACADEMIC PERFORMANCE

-----------------------------------------------

Subject 1 Average:          1.50

Subject 2 Average:          1.75

Overall Grade Average:      1.63


-----------------------------------------------

ACADEMIC RESPONSIBILITIES

-----------------------------------------------

Pending Tasks:              3

Completed Tasks:            5


-----------------------------------------------

ACADEMIC IMPROVEMENT

-----------------------------------------------

Recorded Mistakes:          4

Most Common Category:       Conceptual Errors


-----------------------------------------------

[1] Return to Main Menu

================================================

```


*Note: These are illustrative outputs only, not actual calculations from the provided dataset.*


### Program Flow


```text

              ┌───────────────┐

              │     START     │

              └───────┬───────┘

                      │

                      ▼

          ┌────────────────────────┐

          │ Load JSON Files        │

          └────────────┬───────────┘

                       │

                       ▼

          ┌────────────────────────┐

          │ Display Main Menu      │

          └────────────┬───────────┘

                       │

                       ▼

          ┌────────────────────────┐

          │ Select a Module        │

          └────────────┬───────────┘

                       │

                       ▼

          ┌────────────────────────┐

          │ Perform Selected       │

          │ Operation              │

          └────────────┬───────────┘

                       │

                       ▼

          ┌────────────────────────┐

          │ Validate User Input    │

          └────────────┬───────────┘

                       │

                       ▼

          ┌────────────────────────┐

          │ Save Changes to JSON   │

          │ When Necessary         │

          └────────────┬───────────┘

                       │

                       ▼

                ┌─────────────┐

                │ Exit?       │

                └──────┬──────┘

                       │

                 ┌─────┴─────┐

                 │           │

                NO          YES

                 │           │

                 ▼           ▼

           Return to      ┌─────────┐

           Main Menu      │   END   │

                          └─────────┘

```


## 👥 Task Schedule and Assigned Team Members


| Member | Assigned Responsibilities |

|---|---|

| Emmbert Matthieu O. Cebrian | Student academic records, grade tracker, and grade calculations |

| Rogen Gil R. Tan | Announcement manager, task and deadline manager, and JSON data management |

| Iza Rafaelle T. Corro | Mistake and weakness logger, academic dashboard, and data analysis |


All members will participate in testing, debugging, integration, documentation, and the final presentation.


### Proposed Development Schedule


| Stage | Tasks |

|---|---|

| Week 1 – Planning | Finalize the proposal, inspect the dataset, establish the JSON structures, and design the wireframe |

| Week 2 – Core Development | Implement student records, grade tracking, calculations, and JSON storage |

| Week 3 – Academic Management | Develop announcement management, task management, and mistake logging |

| Week 4 – Analysis and Integration | Implement the academic dashboard, integrate all modules, and perform testing |

| Final Stage | Debug the application, improve the interface, complete documentation, and prepare the presentation |

## 📂 GitHub Repository Link

https://github.com/ircorro2031/StudyTrack.git
