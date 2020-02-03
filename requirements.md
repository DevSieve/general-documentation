
# System Requirements

HR workers and recruiters can create new recruitments, delete existing recruitments.\
There should be an option to send invitation email to candidate ONLY if an exam has been generated.\
There should be an option to send an email to candidate about recruitment result (acceptance or rejection) ONLY if exam sad been finished. 

Recruitment structure:
- candidate's first and last name
- candidate's email
- candidate's CV name (if uploaded)
- difficulty level (junior, mid, senior)
- position (backend, frontend, tester etc)
- exam status
- information on whether the candidate has received an invitation email

HR workers and recruiters can upload/download/delete candidate's CV.\
Cv structure:
- file name
- content

Recruiters can create/update/delete questions that are going to be used to generate an exam for candidate.\
Open question structure:
- question content
- technology
- difficulty level
- time limit
- suggested answer
- max score

Closed question structure:
- question content
- technology
- difficulty level
- time limit
- few closed answers (min 2, max 6), at least one answer must be correct

Recruiters can generate the exam by using a generator or by manually choosing questions from database.\
The generator is going to choose questions based on candidate's skill level and a position that candidate is applying for.\
Recruiters can view created exams independently from current exam's status.\
Recruiters can evaluate open questions in finished exams.\
Recruiters can decide about recruitment acceptance/rejection.\

Exam structure:
- open questions
- closed questions
- max possible score for closed questions
- max possible score for open questions
- time limit
- time left
- status (not started, started, finished, evaluated)

After clicking the link in the invitation email, candidate is moved to the exam execution screen. 
After clicking a 'START' button, the first question appears. System starts counting down time.
Candidate can navigate through all the questions.
The candidate can complete the exam before the time is up.
The exam ends automatically if the time is up.

