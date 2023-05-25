# Problem structure

The files that define a problem are standard for every problem. This approach is suitable for simpler development and is not final. Ideally, a dynamic file structure should be implemented.

## Files that define a problem
```
problem/
├─ README.md            * problem statement
├─ main.cpp             * main problem file
├─ solution_main.cpp    * main problem solution
├─ test0.in             * test input
├─ test1.in
│  ...
├─ test0.ref            * test reference
├─ test1.ref
│  ...
```