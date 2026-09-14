# Azure Project

A Java-based automation testing project using **Selenium WebDriver, TestNG, and Maven**, with an **Azure DevOps CI/CD pipeline** configured to build and test the project automatically.

## Overview

This project demonstrates automated testing using Java and Selenium WebDriver, with TestNG used as the testing framework and Maven used for dependency and build management.

The project also includes an Azure DevOps pipeline configuration that automatically triggers a Maven build when changes are pushed to the `main` branch.

## Key Features

* Java-based automation testing
* Selenium WebDriver integration
* TestNG test framework
* Maven-based project management
* Automated Maven build through Azure DevOps
* JUnit-compatible test result publishing
* CI pipeline triggered on changes to the `main` branch

## Tech Stack

| Technology             | Purpose                            |
| ---------------------- | ---------------------------------- |
| Java 17                | Application and test development   |
| Selenium WebDriver     | Browser automation                 |
| TestNG                 | Test execution and test management |
| Maven                  | Dependency and build management    |
| Azure DevOps Pipelines | Continuous Integration             |
| Git                    | Version control                    |
| IntelliJ IDEA          | Development environment            |

The Maven configuration specifies Java 17 and dependencies for Selenium 4.29.0 and TestNG 7.9.0.

## CI/CD Pipeline

The repository includes an `azure-pipelines.yml` configuration.

The pipeline:

1. Triggers when changes are pushed to the `main` branch.
2. Uses an Ubuntu build agent.
3. Executes the Maven build.
4. Runs the project's tests.
5. Publishes test results from Maven Surefire reports.

The pipeline is configured using Azure DevOps' Maven task.

## Project Structure

```text
azure_project/
│
├── .idea/
├── src/
├── .gitignore
├── azure-pipelines.yml
├── dependency-reduced-pom.xml
├── pom.xml
└── README.md
```

## Getting Started

### Prerequisites

Make sure the following are installed:

* Java JDK 17
* Maven
* Git
* A supported web browser
* Browser driver / Selenium Manager support

### Clone the Repository

```bash
git clone https://github.com/poojakuver535/azure_project.git
```

### Navigate to the Project

```bash
cd azure_project
```

### Build the Project

```bash
mvn clean package
```

### Run Tests

```bash
mvn test
```

## Maven Configuration

The project uses Maven for dependency management and build automation.

The main dependencies include:

* Selenium Java
* TestNG

The project is configured to package the application and generate a runnable JAR with `org.example.Main` as the configured main class.

## Learning Outcomes

Through this project, I practiced:

* Selenium WebDriver automation
* Java-based test development
* TestNG test execution
* Maven dependency management
* Automated build pipelines
* Continuous Integration concepts
* Azure DevOps pipeline configuration

## Future Improvements

* Add more automated test scenarios
* Implement Page Object Model (POM)
* Add explicit waits and reusable utilities
* Generate detailed test reports
* Add cross-browser testing
* Integrate additional CI/CD quality checks
* Add test execution screenshots and documentation

## Author

**Pooja S**

GitHub: https://github.com/poojakuver535

LinkedIn: https://www.linkedin.com/in/pooja-s-79538827/
