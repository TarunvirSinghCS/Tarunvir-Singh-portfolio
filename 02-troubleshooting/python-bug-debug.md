# Python Script Crashed with TypeError

## Problem
A Python script I wrote for data analysis kept crashing with a `TypeError: unsupported operand type(s)` message when processing input files.

## Investigation
- Checked the input files to ensure correct formats.  
- Reviewed the line of code where the error occurred.  
- Added print statements to debug the types of variables.  
- Tested the function with sample inputs to isolate the issue.

## Solution
The error occurred because the code was trying to add a string to an integer. Casting the string to an integer before the operation fixed the problem.

## What I Learned
- Always validate input types before performing operations.  
- Using print statements or a debugger early saves time.  
- Isolating the problem with small test cases helps pinpoint errors faster.

## What Tools Helped
- Python interpreter error messages  
- `print()` debugging  
- VS Code debugger
