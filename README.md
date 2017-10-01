# dailyTasks: A task tracker

DailyTasks is a command line tool that helps keep track of time spent on multiple tasks throughout the day. Tasks are organized by project. You can create a report of the day's time spent on all projects,or a single project.

# Installation and Setup

To use dailyTasks, just put in in your $PATH. There are a few configuration options that you should set up at the top of the script.

# Usage

dt report [regex]    Prints a report based on the regular expression.

dt add [begin] [end] [project] [task]    Adds a new task.

dt rm [task number]    Removes the task with the given number.

dt start [task number]    Changes the start time for the given task number.

dt end [task number]    Changes the end time for the given task number.

dt next [end] [project] [task]    Adds a new task with the same start time as the last task's end time.

dt duration [task number]    Prints the duration of the given task.

dt project [date] [project]    Prints the amount of time worked on the given project for the given date.

dt day [date]    Prints a breakdown of time spent on each project in the given day, with a total for the day.

dt edit    Opens the dailytasks.txt file in an editor.

dt ls    Prints the entire dailytasks.txt file.

Note that times are in the format HH:MM(AM|PM). For single digit hours, the leading zero must be included. For example, to add a task that starts at 10:00 in the morning and ends at 1:00 in the afternoon:

    dt add 10:00AM 01:00PM SomeProject "Developed new module"

In addition, dates are in the format YYYY-MM-DD, so to run a report for a project on December 5, 2016:

    dt project 2016-12-05 SomeProject 

"now" can be used for "begin" and "end" parameters in the add, end, and next actions and the current time will be used.
