DevSieve is a platform for evaluating skills of candidates for the position of web developer. 

### Technology stack:
 - frontend - Angular 8
 - backend -  Java 11, Spring 5, Jpa, Oracle Db, Atmosphere
 - deployment - Heroku
 
## Main use case:

![Main use case](https://github.com/DevSieve/general-documentation/blob/master/main%20use%20case.png)

## Back end side will contain three main services:

### 1. Recruitment Manager
This service will be responsible for:
- creating/deleting recruitments
- creating/deleting exam for candidate based on input parameters such as skill level, technology
- adding/deleting questions and tasks that will be used to generate exam
- evaluating finished exams

### 2. Mail Service
It will be used to send messages to candidate such as: 
- exam invitation
- recruitment acceptance/rejection
- exam results

### 3. Candidate Examination
In this service candidates will solve their exams. To decrease latancy all exams will be kept in memory, users will communicate with service via websockets.

