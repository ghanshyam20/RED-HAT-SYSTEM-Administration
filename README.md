# RED-HAT-SYSTEM-Administration
Red Hat System Administration I (RH124) – Labs, Screenshots, and Notes
# Task 1 – Access the Command Line with the Desktop (RH124)

## Objective
Learn to access the command line using the GNOME 40 desktop environment and perform basic system interactions.

## Key Actions Performed
- Logged in via GNOME graphical interface
- Started lab environment
- Changed user password
- Logged out and verified new password
- Locked and unlocked the session
- Located shutdown option and cancelled
- Finished lab using provided script

## Commands Used
```bash
lab start cli-desktop
passwd
lab finish cli-desktop




# Lab: Access the Command Line (cli-review)

## Overview
This lab focuses on basic interaction with the Linux command line using the Bash shell. The goal of the exercise is to become comfortable running simple commands, identifying file types, viewing file contents, and efficiently reusing commands through shell history and command-line editing.

All tasks were completed as the `student` user on the `workstation` system using the Red Hat training environment.

---

## Lab Preparation
The environment was prepared using the following command:

```bash
lab start cli-review


Commands Executed and Their Purpose
Display current date and time
date


This command displays the current system date and time.

Display time in 24-hour format
date +%R


The +%R format option displays the current time in 24-hour format (HH:MM).

Identify file type
file /home/student/zcat


This command was used to determine the type of the zcat file.
The output confirms that the file is a binary executable and is not human-readable.

Display file size using wc
wc -c /home/student/zcat


The -c option counts the number of bytes in the file, showing the file size.

Bash command history was used to repeat this command efficiently by pressing the up arrow key and executing it again.

Display the first 10 lines of a file
head /home/student/zcat


This command displays the first 10 lines of the specified file.

Display the last 10 lines of a file
tail /home/student/zcat


This command displays the last 10 lines of the file.

The same command was repeated using shell history with minimal keystrokes.

Display the last 20 lines using command-line editing
tail -n 20 /home/student/zcat


This command was created by recalling the previous tail command and editing it to include the -n 20 option, demonstrating efficient command-line editing.

Re-run a previous command using history
date +%R


This command was executed again using the shell history instead of typing it manually.

Lab Evaluation

After completing all tasks, the lab was graded using:

lab grade cli-review


The grading script verified all required actions and returned:

Overall lab grade: PASS

Lab Cleanup

To ensure a clean environment for future exercises, the lab was finalized using:

lab finish cli-review


This command removed temporary files and reset the system state.

Conclusion

This lab provided hands-on practice with essential Bash commands, file inspection tools, and command history shortcuts. All objectives were successfully completed and verified by the automated grading system.

