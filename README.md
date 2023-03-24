# Lab-5_202001431

# Static Analysis of a GitHub Repository

## Information

Repository used for analysis: Tic-Tac-Toe-Minimax  
Link to the repository : https://github.com/Cledersonbc/tic-tac-toe-minimax

File used for analysis: minimax.py  
Link to the file : https://github.com/Cledersonbc/tic-tac-toe-minimax/blob/master/py_version/minimax.py

Tool used for analysis : Pylint  
Link to the tool : https://github.com/PyCQA/pylint

## Tool output:

minimax.py:319:0: C0304: Final newline missing (missing-final-newline) <br/>
minimax.py:1:0: C0114: Missing module docstring (missing-module-docstring) <br/>
minimax.py:8:0: W0105: String statement has no effect (pointless-string-statement) <br/>
minimax.py:62:4: R1703: The if statement can be replaced with 'return bool(test)' (simplifiable-if-statement) <br/>
minimax.py:62:4: R1705: Unnecessary "else" after "return", remove the "else" and de-indent the code inside it (no-else-return) <br/>
minimax.py:85:8: C0103: Variable name "x" doesn't conform to snake_case naming style (invalid-name) <br/>
minimax.py:86:12: C0103: Variable name "y" doesn't conform to snake_case naming style (invalid-name) <br/>
minimax.py:93:15: C0103: Argument name "x" doesn't conform to snake_case naming style (invalid-name) <br/>
minimax.py:93:18: C0103: Argument name "y" doesn't conform to snake_case naming style (invalid-name) <br/>
minimax.py:10:4: R1703: The if statement can be replaced with 'return bool(test)' (simplifiable-if-statement) <br/>
minimax.py:10:4: R1705: Unnecessary "else" after "return", remove the "else" and de-indent the code inside it (no-else-return) <br/>
minimax.py:106:13: C0103: Argument name "x" doesn't conform to snake_case naming style (invalid-name) <br/>
minimax.py:106:16: C0103: Argument name "y" doesn't conform to snake_case naming style (invalid-name) <br/>
minimax.py:113:4: R1705: Unnecessary "else" after "return", remove the "else" and de-indent the code inside it (no-else-return) <br/>
minimax.py:139:8: C0103: Variable name "x" doesn't conform to snake_case naming style (invalid-name) <br/>
minimax.py:139:11: C0103: Variable name "y" doesn't conform to snake_case naming style (invalid-name) <br/>
minimax.py:204:8: C0103: Variable name "x" doesn't conform to snake_case naming style (invalid-name) <br/>
minimax.py:205:8: C0103: Variable name "y" doesn't conform to snake_case naming style (invalid-name) <br/>
minimax.py:208:8: C0103: Variable name "x" doesn't conform to snake_case naming style (invalid-name) <br/>
minimax.py:208:11: C0103: Variable name "y" doesn't conform to snake_case naming style (invalid-name) <br/>
minimax.py:248:12: R1722: Consider using 'sys.exit' instead (consider-using-sys-exit) <br/>
minimax.py:263:10: R1714: Consider merging these comparisons with 'in' by using 'h_choice not in ('O', 'X')'. Use a set instead if elements are hashable. (consider-using-in) <br/>
minimax.py:269:12: R1722: Consider using 'sys.exit' instead (consider-using-sys-exit) <br/>
minimax.py:281:10: R1714: Consider merging these comparisons with 'in' by using 'first not in ('Y', 'N')'. Use a set instead if elements are hashable. (consider-using-in) <br/>
minimax.py:286:12: R1722: Consider using 'sys.exit' instead (consider-using-sys-exit) <br/>
minimax.py:315:4: R1722: Consider using 'sys.exit' instead (consider-using-sys-exit) <br/>
minimax.py:253:0: R0912: Too many branches (13/12) (too-many-branches) <br/>

-----------------------------------
Your code has been rated at 8.27/10

## Understanding tool output

### C0304: Final newline missing
A newline should be printed at the end of the file for better readability of I/O.

### C0114: Missing module docstring
A Python module should have a docstring, explaining what the module does, what it provides, and examples of how to use the classes, methods, and functions.

### R1703: The if statement can be replaced with 'return bool(test)'
Code should avoid using if statements, if the work can be achieved thorugh simple return statements.

### R1705: Unnecessary "else" after "return", remove the "else" and de-indent the code inside it
Code should avoid using a else after a block of ifs, if all of them consist of an return statement.

### R1722: Consider using 'sys.exit' instead
Pylint suggests using sys.exit since, compared to 'exit()' or 'quit()', it does not rely on the site module being available (as the 'sys' module is always available).

### R0912: Too many branches (13/12)
Pylint suggests at max 12 branches. The code has exceeded this limit.


