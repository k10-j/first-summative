The Submission Reminder App is a simple yet effective tool designed to help track student assignment submissions. It automates the process of checking which students have not submitted their assignments and provides timely reminders.

Key Functions:
Setup and Configuration

The app creates a personalized environment for the user, generating necessary files and directories.
It stores assignment details and deadlines in a configuration file (config.env).
Users can add new student records during setup.
Submission Tracking

The app maintains a database (submissions.txt) listing students, their assignments, and submission statuses.
When executed, it scans this file and identifies students who haven't submitted their work.
Automated Reminders

The app prints reminders for students with pending assignments.
It provides information on the assignment name and remaining submission days.
User-Friendly Execution

The startup.sh script ensures all necessary files exist before running the reminder tool.
The reminder.sh script processes student records and displays reminders.
Example Use Case
Imagine a teacher or course administrator wants to track assignment submissions. Instead of manually checking records, they can run the Submission Reminder App, which will:

Read the list of student submissions.
Identify those who have not yet submitted.
Display a reminder message for each pending submission.
This simple automation saves time and ensures that students are consistently reminded of their deadlines.
# first-summative
