dt report [regex]
    Prints a report based on the regular expression.

dt add [begin] [end] [project] [task]
    Adds a new task.

dt rm [task number]
    Removes the task with the given number.

dt start [task number]
    Changes the start time for the given task number.

dt end [task number]
    Changes the end time for the given task number.

dt next [end] [project] [task]
    Adds a new task with the same start time as the last task's end time.

dt duration [task number]
    Prints the duration of the given task.

dt project [date] [project]
    Prints the amount of time worked on the given project for the given date.

dt day [date]
    Prints a breakdown of time spent on each project in the given day, with a total for the day.

dt edit
    Opens the dailytasks.txt file in an editor.

dt ls
    Prints the entire dailytasks.txt file.

"now" can be used for "begin" and "end" parameters in the add, end, and next actions.
