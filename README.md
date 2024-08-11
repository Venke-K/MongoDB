#Task 1 

MongoDB task using the provided JSON data we need to fetch some using the Command


For the following question write the corresponding MongoDB queries

Find all the information about each products
Find the product price which are between 400 to 800
Find the product price which are not between 400 to 600
List the four product which are greater than 500 in price 
Find the product name and product material of each products
Find the product with a row id of 10
Find only the product name and product material
Find all products which contain the value of soft in product material 
Find products which contain product color indigo  and product price 492.00
Delete the products which product price value are 28

##Task2 

MongoDB Database Design for Zen Class Program

Here's a sample README for the MongoDB Database Design for the Zen Class Program:
MongoDB Database Design for Zen Class Program
Overview

This project outlines the database design for the Zen Class Program, focusing on managing user attendance, task submissions, and mentoring activities. The design uses MongoDB as the database management system to efficiently handle the data related to users, tasks, attendance, topics, company drives, and mentors.
Collections

The following collections are included in the database design:

   Users Collection
   Fields:
   user_id: Unique identifier for each user.
   name: Name of the user.
   email: Email address of the user.
   role: Role of the user (e.g., student, mentor).

  Codekata Collection
   Fields:
   user_id: Unique identifier for the user.
   problems_solved: Number of problems solved by the user.
   submission_date: Date of submission.

   Attendance Collection
   Fields:
   user_id: Unique identifier for the user.
  date: Date of attendance.
   status: Attendance status (e.g., present, absent).

  Topics Collection
  Fields:
  topic_id: Unique identifier for each topic.
  name: Name of the topic.
  description: Description of the topic.

  Tasks Collection
   Fields:
   task_id: Unique identifier for each task.
   user_id: Unique identifier for the user.
   due_date: Due date for the task.
   status: Submission status (e.g., submitted, not submitted).

   Company Drives Collection
   Fields:
   drive_id: Unique identifier for each company drive.
   company_name: Name of the company.
   date: Date of the drive.
   location: Location of the drive.

   Mentors Collection
   Fields:
   mentor_id: Unique identifier for each mentor.
   name: Name of the mentor.
   mentees: Array of user_ids for mentees associated with the mentor.

Relationships

   Each user can have multiple tasks and attendance records.
   Each task is associated with a user.
   Each mentor can have multiple mentees.
   Company drives are independent records but can be linked to users who participate.
