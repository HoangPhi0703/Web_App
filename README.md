# Web_App

Link to open the app: https://db2.fb2.frankfurt-university.de/ords/r/vgu2425_02/waasac190179/home?session=0

# Project – Group 2

## Group Members

- Muhammad Bilal Javed - 21I-0584
- Muhammad Taimoor - 21I-0611
- Jawad Ahmed - 21I-2489
- Zaid Shahid - 21I-2465
- Hassan Waseem - 21I-0883
- Muhammad Hamza - 21I-0597

---

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

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/quiz-voting-system.git
    ```

2. Set up Oracle APEX workspace.

3. Import database schema and tables provided in the `/database` folder.

4. Launch the APEX application and start using the platform.

---

## Future Enhancements

- Add quiz timer and session expiration.
- Export quiz reports to PDF.
- Implement question difficulty tagging.
- Improve UI with modern CSS framework.

---

## Screenshots

(Add screenshots of your app pages here in markdown like below)

```markdown
![Login Page](screenshots/login.png)
![Dashboard](screenshots/dashboard.png)
![Quiz Page](screenshots/quiz.png)

