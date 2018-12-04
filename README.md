# chalk

Chalk is a line based text editor for the terminal. It was originally developed for _colorsh_ a custom shell used for ssh accounts on the developers server. It has been split out here as its own application.

### Install

Requires Python 3.6+. No other Python dependencies, standard library only.
Copy the file `chalk` to anywhere on your system path (or add it to your system path).
You should now be able to run chalk with the following command:
`chalk /path/to/file.txt`
The above command will open a file if a valid one is found at the path, or it will create one.


### Commands

Commands are entered as the only text on their row. Enter the command and press enter.

.  - Finish editing and, optionally, save. Then exit.

!d - Display all text in the document

!x - Delete line(s). If one number is entered, that line will be removed. 
         If two numbers separated by a space are entered, a range inclusive 
         of both numbers will be removed.

!i - Insert line(s) after the first line number entered. A second number
         separated from the first by a space can be included to as a count
         of how many lines to insert.

!# - Edit a line, where # is the line number. E.g. `> !23`

!? - View this list of available commands

### Notes

This application uses the python readline library to allow for common terminal based hotkeys (ex. C-a to go to the beginning of the line). It also provides a convenient history that is accessible via up and down arrows.

