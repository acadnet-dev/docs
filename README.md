# Documentation for acadnet.dev project
This repo is a starting point for writing my diploma thesis. It contains all the documentation for the project.

## Project idea
To better understand the idea behind the project please start with the [user journey](docs/user-journey.md). You should also check the [software architecture](docs/software-architecture.md) stack.

## Problem listing and structure
For listing the problems I have gone with a dynamic recursive structure of categories that can hold other categories or problems as children. Check the [problem hierarchy](docs/problem-hierarchy.md) for more details.

For the problem structure I have went with a pre-defined standard, even though a dynamic one will be implemented for the final product. See the [problem structure](docs/problem-structure.md) doc.

## Checker
The checker is written in Python as a standalone endpoint. Here is the [checker documentation](docs/checker-api.md).

## So you want to create a problem?
Check the [problem author](docs/problem-author.md) doc.

## Docs
* [User journey](docs/user-journey.md) - describes the user journey through the app
* [Software architecture](docs/software-architecture.md) - describes the software architecture of the app
* [Problem hierarchy](docs/problem-hierarchy.md) - describes the courses and problems layout
* [Problem structure](docs/problem-structure.md) - describes a problem structure (files)
* [Checker documentation](docs/checker.md) - describes the checker architecture and how it works
* [Checker API](docs/checker-api.md) - describes the API that the checkers exposes
* [Problem author](docs/problem-author.md) - describes how to create a problem

## Timeline
```mermaid
gantt
    title Timeline acadnet.dev
    axisFormat %d-%b
    section Dev
    Project startup                                     :done, a0, 2023-05-07, 15d
    Problem struct + statement + example                :active, a1, 2023-05-22, 5d
    Checker + upload submission page + results page     :a11, after a1, 1w
    VSCode workspace for students                       :a12, after a11, 3d
    VSCode extension for checking                       :a13, after a12, 5d
    Add more problems + final checks                    :after a13, 1w
    section Ops
    Setup CI/CD + deploy to DO                          :a2, 2023-06-01, 1w
    section Documentation
    Write docs                                          :a3, 2023-06-12, 22d
```

## How to edit the docs
* To edit the diagrams you need to install this vscode extension: [Draw.io Integration](https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio)