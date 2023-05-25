# Problem structure

The files that define a problem are standard for every problem. This approach is suitable for simpler development and is not final. Ideally, a dynamic file structure should be implemented.

## Files that define a problem
```
problem/
├─ README.md            * problem statement
├─ main.cpp             * main problem file
├─ solution_main.cpp    * main problem solution
├─ tests/               * folder with tests
│  ├─ in/               * input for each test
│  │  ├─ test0.in
│  │  ├─ test1.in
│  │  ...
│  ├─ ref/              * correct output for each test
│  │  ├─ test0.ref
│  │  ├─ test1.ref
│  │  ...

```