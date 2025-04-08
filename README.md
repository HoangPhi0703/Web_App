# Web_App

Link to open the app: https://db2.fb2.frankfurt-university.de/ords/r/vgu2425_02/waasac190179/home?session=0


## Project Title: Quiz and Voting System

### Project Description

The Quiz and Voting System is a web-based platform designed to facilitate the creation and administration of quizzes. It also includes features for evaluating and rating free-text questions through a voting mechanism.

---

## Key Features

- User-friendly web interface for quiz creation and participation.
- Support for multiple-choice and free-text questions.
- Real-time feedback and evaluation of responses.
- Voting system for rating free-text questions post-quiz.

---

## Tools and Technologies

- **Database:** Oracle APEX
- **Frontend:** APEX Web UI
- **Backend:** PL/SQL (Oracle APEX)
- **Languages:** SQL, PL/SQL
- **Version Control:** Git & GitHub

---

## Application Screens Overview

### 1. Login Page
- User authentication based on student ID.
- Redirects to dashboard after successful login.

### 2. Dashboard
- Displays a summary of user-created and participated quizzes.
- Options to create new quizzes.

### 3. Quiz Creation Page
- Input quiz title, description, and questions.
- Add answers and mark correct options for MCQs.

### 4. Quiz Play Page
- Users participate in quizzes.
- Timer functionality and submission handling.

### 5. Evaluation Page
- Shows correct answers and user responses.
- Calculates total score and displays it.

### 6. Voting Page
- Displays free-text questions.
- Users rate each question on a scale of 1 to 5.

---

## Database Tables

### USERS
| Column Name | Description      |
|-------------|------------------|
| USERID      | Primary Key      |
| NAME        | User’s full name |
| EMAIL       | User’s email     |

### QUIZZES
| Column Name | Description        |
|-------------|--------------------|
| QUIZID      | Primary Key        |
| TITLE       | Quiz title         |
| USERID      | Creator’s user ID  |

### QUESTIONS
| Column Name | Description             |
|-------------|-------------------------|
| QUESTIONID  | Primary Key             |
| QUIZID      | Foreign Key             |
| TEXT        | Question text           |
| TYPE        | 'MC' or 'SA' (short answer) |

### ANSWERS
| Column Name | Description                  |
|-------------|------------------------------|
| ANSWERID    | Primary Key                  |
| QUESTIONID  | Foreign Key                  |
| TEXTANS     | Text of the answer           |
| ANSWERTYPE  | 'MC' for multiple choice, 'SA' for short answer |

### VOTES
| Column Name | Description      |
|-------------|------------------|
| VOTEID      | Primary Key      |
| QUESTIONID  | Foreign Key      |
| RATING      | Value (1 to 5)   |

---

## How to Run the Project

Because this is a External Project in a Private Oracle Apex workspace so you need permission to view all the project. However to run the application you just need to click thẻ link at the beginning of this file.

## Future Enhancements

- Add quiz timer and session expiration.
- Export quiz reports to PDF.
- Implement question difficulty tagging.
- Improve UI with modern CSS framework.

---



