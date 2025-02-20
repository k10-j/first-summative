# Submission Reminder App 
The Submission Reminder App is a simple yet effective tool designed to help track student assignment submissions. It automates the process of checking which students have not submitted their assignments and provides timely reminders. 

## Overview  
The **Submission Reminder App** is a Bash-based tool designed to track and remind students of pending assignment submissions. It automates the process of managing submissions, ensuring that no student misses their deadlines.  

## Features  
 **Automated setup** – Creates all necessary directories and files.  
 **Submission tracking** – Identifies students who haven't submitted their assignments.  
 **Configurable reminders** – Users can define assignments and deadlines.  
 **User-friendly execution** – Simple commands to set up and run the app.  

## Setup Instructions  

### 1. Run the Setup Script  
Execute the following command to set up the environment:  
```bash
bash setup.sh
```
This script will:  
 Ask for a username (ensuring only valid characters).  
 Create a directory `submission_reminder_<username>` with subdirectories (`assets`, `config`, `modules`).  
 Generate required configuration and script files.  
 Allow the user to add five student records.  
 Make the scripts executable.  

### 2. Start the Application  
Once setup is complete, navigate to the directory and run:  
```bash
cd submission_reminder_<username>  
./startup.sh
```
The startup script:  
- Verifies required files exist.  
- Ensures scripts are executable.  
- Runs the **submission reminder** tool.  

## How It Works  

1. The app stores **assignment details** and deadlines in `config.env`.  
2. It maintains a **student submissions database** in `submissions.txt`.  
3. When `reminder.sh` runs, it checks for students who **haven't submitted** their assignments.  
4. It prints reminders listing students and their pending assignments.  

## File Structure  

```
submission_reminder_<username>/
│── assets/
│   ├── submissions.txt      # Student submission records
│── config/
│   ├── config.env           # Stores assignment details
│── modules/
│   ├── functions.sh         # Helper functions for processing submissions
│── reminder.sh              # Core script to check submissions
│── startup.sh               # Main script to launch the app
```

## Example Output  

```bash
Assignment: Shell Navigation  
Days remaining to submit: 2 days  
--------------------------------------------  
Reminder: Chinemerem has not submitted the Shell Navigation assignment!  
Reminder: Divine has not submitted the Shell Navigation assignment!  
```

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
