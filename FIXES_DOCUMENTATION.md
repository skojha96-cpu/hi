# BUG FIXES DOCUMENTATION

This document outlines all the bugs found in the exam management system and their corresponding fixes. Each entry includes the bug description, steps to reproduce, the fix implemented, and any additional notes.

## Bug List

### 1. Bug: User Unable to Submit Exam
**Description:** Users reported that they were unable to submit their exam after completing it.
- **Steps to Reproduce:**  
  1. Log in as a student.  
  2. Start an exam.  
  3. Complete the exam and attempt to submit.  
- **Fix Implemented:**  
  Corrected the form submission logic to ensure that the `submit` button was properly enabled after the exam completion.
- **Date Fixed:** 2026-02-15

### 2. Bug: Incorrect Grading for Multiple Choice Questions
**Description:** The system was marking multiple choice answers incorrectly.
- **Steps to Reproduce:**  
  1. Assign a multiple choice exam.  
  2. Answer questions and submit.  
- **Fix Implemented:**  
  Reviewed the answer checking logic to ensure that the correct answers were matched correctly.
- **Date Fixed:** 2026-03-01

### 3. Bug: Scheduled Exams Not Appearing in Student Dashboard
**Description:** Some scheduled exams were not visible to students in their dashboard.
- **Steps to Reproduce:**  
  1. Log in as a student.  
  2. Observe the list of scheduled exams.
- **Fix Implemented:**  
  Adjusted the query that fetches exams to include all scheduled exams for the current period.
- **Date Fixed:** 2026-02-25

### 4. Bug: System Crash on Exam Start
**Description:** The application crashes when a student tries to start an exam.
- **Steps to Reproduce:**  
  1. Log in as a student.  
  2. Start an exam.  
- **Fix Implemented:**  
  Implemented error handling around the exam start process to prevent crashes. 
- **Date Fixed:** 2026-03-10

### 5. Bug: Inability to Reset Password
**Description:** Users could not reset their passwords due to a broken link.
- **Steps to Reproduce:**  
  1. Go to the login page.
  2. Click on ‘Forgot Password’ link.
- **Fix Implemented:**  
  Fixed the URL for the password reset link.
- **Date Fixed:** 2026-03-15

## Additional Notes
- Ensure thorough testing after applying fixes to prevent regression.
- Maintain clear documentation for future reference and audits.