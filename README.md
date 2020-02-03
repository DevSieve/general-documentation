DevSieve is a platform for evaluating skills of candidates for the position of web developer. 

### Technology stack:
 - frontend - Angular 8
 - backend -  Java 11, Spring 5, Jpa, Oracle Db, Atmosphere
 - deployment - Heroku
 
## Main use case:

![Main use case](https://github.com/DevSieve/general-documentation/blob/master/main%20use%20case.png)

## Back end side is going to have three microservices:

### 1. Recruitment Manager
This service is going to be responsible for:
- creating/deleting recruitments
- creating exam for candidate based on parameters such as skill level, technology
- adding/deleting questions and tasks that will be used to generate exam
- evaluating finished exams

### 2. Mail Service
It is going to be used for sending messages to candidate such as: 
- exam invitation
- recruitment acceptance/rejection
- exam results

### 3. Candidate Examination
In this service candidates will be solvingfa their exams. To decrease latancy all exams will be kept in memory, users will communicate with service via websockets.


# System Requirements

HR workers and recruiters can create new recruitments, delete existing recruitments.
Recruitment structure:
- candidate's first and last name
- candidate's gender
- candidate's email
- candidate's CV name (if uploaded)
- difficulty level (junior, mid, senior)
- position (backend, frontend, tester etc)
- exam status



HR workers and recruiters can upload/download candidate's CV.
Cv structure:
- file name
- content



Recruiters can create/update/delete questions that are going to be used to generate an exam for candidate.
Open question structure:
- question content
- technology
- difficulty level
- time limit
- suggested answer

Closed question structure:
- question content
- technology
- difficulty level
- time limit
- few closed answers (min 2, max 6) - at least one answer must be correct



Recruiters can generate the exam by using a generator or by manually choosing questions from database.
The generator is going to choos questions based on candidate's skill level and position.
Recruiters can view created exams independently from current exam's status.
Recruiters can evaluate open questions in finished exams.
Recruiters can decide about recruitment acceptance/rejection

Exam structure:
- open questions
- closed questions
- max possible score for closed questions
- max possible score for open questions
- time limit
-time left
- status (not started, started, finished, evaluated)

