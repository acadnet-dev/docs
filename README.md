# Documentation for acadnet.dev project
This repo is a starting point for writing my diploma thesis. It contains all the documentation for the project.

## Project idea
To better understand the idea behind the project please start with the [user journey](docs/user-journey.md). You should also check the [software architecture](docs/software-architecture.md) stack.

## Docs
* [User journey](docs/user-journey.md) - describes the user journey through the app
* [Software architecture](docs/software-architecture.md) - describes the software architecture of the app

## Timeline
```mermaid
gantt
    title Timeline acadnet.dev
    axisFormat %d-%b
    section Dev
    Problem struct + statement + example                :a1, 2023-05-22, 5d
    Checker + upload submission page + results page     :after a1, 1w
    section Ops
    Setup CI/CD + deploy to DO                          :a2, 2023-06-01, 5d
    section Documentation
    Start writing docs                                  :a3, 2023-06-12, 2023-06-24
    Final checks                                        :after a3, 2d
```

## How to edit the docs
* To edit the diagrams you need to install this vscode extension: [Draw.io Integration](https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio)