# Software Engineering Lab Assignments

<p align="center">

  **PES University | Department of Computer Science and Engineering**

  **Course:** UE24CS341A – Software Engineering

  **Academic Year:** 2026–2027

  **Semester:** 5th Semester

</p>

---

## Student Information

| Field | Details |
|---|---|
| Student Name | Pratham Kumar |
| SRN | PES2UG24CS368 |
| PRN | PES2202400086 |
| University | PES University |
| Course | UE24CS341A – Software Engineering |
| Academic Year | 2026–2027 |

---

## 1. Repository Overview

This repository contains the collection of seven Software Engineering laboratory assignments completed as part of the UE24CS341A – Software Engineering course at PES University.

The assignments provide practical experience in different phases and activities of software engineering, including requirements engineering, Agile project management, software architecture, debugging, static code analysis, software testing, code coverage measurement, and fuzz testing.

The repository is organized into seven individual lab folders. Each folder contains its corresponding README documentation and the available assignment deliverables, such as completed lab reports, instructor-provided handouts, supporting documents, and external GitHub project references.

For assignments implemented in separate GitHub repositories, the corresponding folder contains a `GitHub_Link.txt` file that provides direct access to the complete implementation.

---

## 2. Laboratory Assignments

### Lab 01 – Requirements Engineering & UML Use-Case Modelling

**Objective:** To analyse an instructor-provided problem scenario, identify system requirements, define acceptance criteria, identify actors, and represent system functionality through UML Use-Case Modelling.

**Project Scenario:** Podcast Guest Scheduling & Outline Builder.

**Work Completed:**
- Analysed the assigned problem statement.
- Identified three primary actors: Podcast Guest, Show Host, and Calendar Service.
- Identified five Functional Requirements (FR-001 to FR-005).
- Defined two Non-Functional Requirements (NFR-001 and NFR-002).
- Documented priorities and measurable acceptance criteria.
- Prepared a UML Use-Case Diagram.
- Defined `include` and `extend` relationships.
- Prepared a detailed Use-Case Flow Specification for booking an interview slot, including the main success scenario and alternate flow.

**Key Concepts:** Requirements Elicitation, Functional Requirements, Non-Functional Requirements, Acceptance Criteria, UML Use-Case Diagrams, Actors, and Use-Case Flows.

**Folder:** [`Lab-01/`](Lab-01/)

---

### Lab 02 – Agile Backlog Creation & Sprint Simulation in Jira

**Objective:** To apply Agile project management practices by converting requirements into Epics and User Stories, organizing a Product Backlog, estimating effort, and simulating Scrum sprint execution using Jira.

**Project Scenario:** Podcast Guest Scheduling & Outline Builder.

**Work Completed:**
- Created a Company-managed Scrum project in Jira.
- Created four Epics.
- Developed nine User Stories.
- Organized and prioritized the Product Backlog.
- Estimated work using Fibonacci Story Points.
- Studied Planning Poker as an estimation technique.
- Planned and executed two simulated sprints.
- Used Jira's Active Sprint board to monitor task progress.
- Analysed Sprint Reports and Burndown Charts.

**Sprint Results:**

| Metric | Sprint 1 | Sprint 2 |
|---|---:|---:|
| User Stories | 3 | 6 |
| Planned Story Points | 13 | 20 |
| Completed Story Points | 13 | 20 |

**Total:** 9 User Stories and 33 Story Points.

**Key Concepts:** Agile Methodology, Scrum, Jira, Product Backlog, Epics, User Stories, Story Point Estimation, Sprint Planning, and Burndown Charts.

**Folder:** [`Lab-02/`](Lab-02/)

---

### Lab 03 – Component Modelling & Architectural Pattern Selection

**Objective:** To analyse different software architectural styles, select a suitable architecture for the assigned system, and understand UML Component Modelling concepts.

**Project Scenario:** Podcast Guest Scheduling & Outline Builder.

**Work Completed:**
- Studied Layered Architecture.
- Evaluated Microservices Architecture.
- Evaluated Client-Server Architecture.
- Compared architectural advantages and limitations.
- Selected Layered Architecture for the assigned scenario.
- Justified the selection based on separation of responsibilities, system scope, security, and performance.
- Studied UML Component Diagram notation.
- Examined components, provided interfaces, required interfaces, ports, dependencies, and assembly connectors.

**Selected Architecture:** Layered Architecture.

**Logical Layers:**
1. Presentation Layer.
2. Business Layer.
3. Data Layer.

**Key Concepts:** Software Architecture, Architectural Pattern Selection, Layered Architecture, Microservices, Client-Server Architecture, UML Component Diagrams, Interfaces, and Dependencies.

**Folder:** [`Lab-03/`](Lab-03/)

---

### Lab 04 – Number Guessing Game Repair

**Objective:** To debug and enhance an existing Python-based Number Guessing Game by correcting input-handling defects and implementing additional gameplay features.

**Project:** Number Guessing Game – Pygame Edition.

**Work Completed:**
- Identified and fixed the empty-input crash.
- Implemented input validation before integer conversion.
- Added dynamic minimum and maximum search-range display.
- Implemented a recent guess history panel displaying the last five guesses.
- Added colour-coded feedback for TOO HIGH, TOO LOW, and CORRECT.
- Introduced a maximum limit of ten attempts.
- Implemented a Game Over state that reveals the secret number.
- Added a restart option using the R key.

**Technologies:** Python, Pygame.

**External Implementation Repository:**

[60_number_guess](https://github.com/PKumar041104/60_number_guess)

The complete source code and implementation are maintained in the external repository. The `Lab-04/GitHub_Link.txt` file provides the direct repository reference.

**Key Concepts:** Debugging, Input Validation, Exception Prevention, State Management, Conditional Logic, and Modular Programming.

**Folder:** [`Lab-04/`](Lab-04/)

---

### Lab 05 – Static Code Analysis: Student Attendance Tracker

**Objective:** To improve the security, quality, reliability, and maintainability of an existing Python application using static code analysis tools.

**Project:** Student Attendance Tracker.

**Tools Used:**
- Pylint – Code Quality Analysis.
- Bandit – Security Analysis.
- Flake8 – Coding Standard Analysis.

**Work Completed:**
- Analysed the original Attendance Tracker application.
- Identified security vulnerabilities and functional issues.
- Corrected disabled TLS certificate verification.
- Removed hard-coded API-key configuration.
- Replaced shell-based archive creation with Python's `tarfile` module.
- Added HTTP request timeouts and response validation.
- Fixed mutable default arguments.
- Corrected attendance eligibility boundary conditions.
- Handled division-by-zero risks.
- Prevented duplicate attendance records.
- Improved date validation and CSV export safety.
- Improved resource handling, documentation, and coding standards.
- Executed all three static analysis tools again after applying corrections.

**Recorded Results:**

| Tool | Initial Result | Final Result |
|---|---|---|
| Pylint | 4.55/10 | 10.00/10 |
| Bandit | 8 findings | 0 findings |
| Flake8 | Multiple violations | 0 violations |

**Key Concepts:** Static Code Analysis, Security Vulnerability Detection, Code Quality, PEP 8, Input Validation, Secure Programming, and Maintainability.

**External Implementation Repository:**

[L5_61_attendance-tracker](https://github.com/PKumar041104/L5_61_attendance-tracker)

The complete implementation, issue analysis, and supporting evidence are maintained in the external repository.

**Folder:** [`Lab-05/`](Lab-05/)

---

### Lab 06 – Code and Branch Coverage Analysis

**Objective:** To evaluate the completeness of automated software testing using statement coverage and branch coverage techniques.

**Project:** Marathon Registration Application.

**Technologies and Tools:**
- Python 3.14.0.
- pytest 9.2.0.
- coverage.py 7.17.0.

**Work Completed:**
- Analysed the Marathon Registration application.
- Extended the starter test suite.
- Created additional code-coverage test cases.
- Created additional branch-coverage test cases.
- Tested normal inputs and boundary conditions.
- Executed automated tests using pytest.
- Measured statement and branch coverage using coverage.py.
- Verified uncovered statements and branches.

**Recorded Results:**

| Metric | Result |
|---|---:|
| Code-Coverage Test Cases Passed | 35 |
| Line Coverage | 100% |
| Branch-Coverage Test Cases Passed | 28 |
| Branch Coverage | 100% |
| Missing Statements | 0 |
| Missing Branches | 0 |

**Key Concepts:** Software Testing, Statement Coverage, Branch Coverage, Automated Testing, pytest, coverage.py, and Test-Case Design.

**Shared External Implementation Repository:**

[L6_L7_60_marathon_registration](https://github.com/PKumar041104/L6_L7_60_marathon_registration)

Refer to the `LAB6` directory in the external repository for the Lab-06 implementation, test suites, and supporting evidence.

**Folder:** [`Lab-06/`](Lab-06/)

---

### Lab 07 – Fuzzing for Input Validation Bugs

**Objective:** To identify and correct input-validation defects using fuzz testing and property-based testing with the Hypothesis framework.

**Project:** Marathon Registration Parser.

**Technologies and Tools:**
- Python 3.14.0.
- Hypothesis 6.170.15.
- pytest 9.2.0.

**Work Completed:**
- Analysed the original Marathon Registration Parser.
- Studied the behaviour of three primary functions:
  - `format_bib_name()`
  - `parse_finish_time()`
  - `average_split()`
- Completed the provided Hypothesis test template.
- Generated unexpected and malformed inputs automatically.
- Identified AttributeError, ValueError, and ZeroDivisionError.
- Implemented defensive programming and input validation.
- Added checks for input types, empty values, numeric formats, and valid time ranges.
- Re-executed the same test suite against the corrected application.

**Recorded Results:**

| Testing Stage | Result |
|---|---|
| Original Application | 3 Failed |
| Corrected Application | 3 Passed |

**Key Concepts:** Fuzz Testing, Property-Based Testing, Hypothesis, pytest, Input Validation, Exception Handling, and Defensive Programming.

**Shared External Implementation Repository:**

[L6_L7_60_marathon_registration](https://github.com/PKumar041104/L6_L7_60_marathon_registration)

Refer to the `LAB7` directory in the external repository for the Lab-07 implementation, Hypothesis test suite, screenshots, and supporting evidence.

**Folder:** [`Lab-07/`](Lab-07/)

---

## 3. Repository Structure

The repository is organized into seven individual laboratory directories.

```text
Software-Engineering-Lab-Assignments-PES2UG24CS368/
│
├── README.md
│
├── Lab-01/
│   ├── README.md
│   ├── 60_SE_Lab1_SE_Problem_Statements.pdf
│   ├── Student_guidelines.pdf
│   └── PES2UG24CS368-PRATHAM_KUMAR-LAB_1.pdf
│
├── Lab-02/
│   ├── README.md
│   ├── Lab_2_Jira_Student_Handout.pdf
│   └── PES2UG24CS368_PRATHAM-KUMAR_Lab2_Jira.pdf
│
├── Lab-03/
│   ├── README.md
│   ├── Lab_3_Architecture_Student_handout.pdf
│   └── PES2UG24CS368_PRATHAM-KUMAR_Lab3-UML_Component_Diagram.pdf
│
├── Lab-04/
│   ├── README.md
│   └── GitHub_Link.txt
│
├── Lab-05/
│   ├── README.md
│   ├── GitHub_Link.txt
│   ├── Lab_5_Static_Code_Analysis_Student_handout.pdf
│   └── Lab_5_Static_Code_Analysis_Student_handout.docx
│
├── Lab-06/
│   ├── README.md
│   └── [Lab-06 deliverables and GitHub reference]
|   └── Lab_6_Code&BranchCoverage_Student_Handout.docx
|   └── PES2UG24CS368-LAB6-Code&BranchCoverage
│
└── Lab-07/
    ├── README.md
    ├── GitHub_Link.txt
    ├── Lab_7_FuzzTesting_Student_Handout.pdf
    └── PES2UG24CS368-LAB7.pdf
```

*Note: The directory listing above represents the intended logical organization. Consult the individual lab folders for the actual available files.*

---

## 4. External GitHub Project References

Some laboratory assignments involve practical implementations maintained in separate GitHub repositories.

| Laboratory | External Project | Repository |
|---|---|---|
| Lab 04 | Number Guessing Game Repair | [60_number_guess](https://github.com/PKumar041104/60_number_guess) |
| Lab 05 | Static Code Analysis – Attendance Tracker | [L5_61_attendance-tracker](https://github.com/PKumar041104/L5_61_attendance-tracker) |
| Lab 06 | Code and Branch Coverage Analysis | [L6_L7_60_marathon_registration](https://github.com/PKumar041104/L6_L7_60_marathon_registration) |
| Lab 07 | Fuzzing for Input Validation Bugs | [L6_L7_60_marathon_registration](https://github.com/PKumar041104/L6_L7_60_marathon_registration) |

**Note:** Lab-06 and Lab-07 share the same external GitHub repository, with their implementations maintained separately in the `LAB6` and `LAB7` directories.

For Lab-04 through Lab-07, the individual `GitHub_Link.txt` files provide the corresponding repository references.

---

## 5. Tools and Technologies Summary

The following tools and technologies were used across the seven laboratory assignments.

| Category | Tools / Technologies |
|---|---|
| Requirements Engineering | UML Use-Case Modelling |
| Agile Project Management | Jira, Scrum |
| Software Architecture | Layered Architecture, UML Component Modelling |
| Programming | Python |
| Game Development | Pygame |
| Static Code Analysis | Pylint, Bandit, Flake8 |
| Automated Testing | pytest |
| Code Coverage | coverage.py |
| Fuzz Testing | Hypothesis |
| Version Control | Git |
| Repository Hosting | GitHub |

---

## 6. Overall Learning Outcomes

The seven laboratory assignments provided practical exposure to the software engineering lifecycle and different software quality assurance techniques.

The major learning outcomes include:

1. Understanding how to translate real-world problem statements into structured software requirements.
2. Preparing functional and non-functional requirements with measurable acceptance criteria.
3. Applying Agile methodologies and Scrum practices using Jira.
4. Understanding architectural styles and selecting suitable software architectures.
5. Modelling software components and their interactions using UML.
6. Debugging existing applications and implementing functional enhancements.
7. Identifying security vulnerabilities and code-quality issues through static analysis.
8. Designing automated tests and measuring statement and branch coverage.
9. Using property-based fuzz testing to identify unexpected input-handling defects.
10. Applying defensive programming and input-validation techniques.
11. Maintaining source code, documentation, and project deliverables using Git and GitHub.

---

## 7. How to Navigate This Repository

- Open the respective `Lab-01` through `Lab-07` folder to explore an individual assignment.
- Read the folder-level `README.md` for the objective, implementation details, tools, results, and learning outcomes.
- Refer to the included PDF documents for instructor guidelines and completed lab reports.
- For assignments implemented in external repositories, open the corresponding `GitHub_Link.txt` file or use the direct repository link provided in the README.
- For Lab-06 and Lab-07, navigate to the respective `LAB6` and `LAB7` directories in their shared external repository.

---

## 8. Conclusion

This repository presents the complete collection of seven Software Engineering laboratory assignments completed as part of the UE24CS341A course at PES University.

The assignments cover a broad range of software engineering practices, beginning with requirements engineering and Agile project planning, progressing through software architecture and debugging, and extending into static analysis, automated testing, code coverage, and fuzz testing.

Together, these experiments demonstrate the practical application of software engineering principles, development tools, testing methodologies, and quality assurance techniques throughout the software development lifecycle.

---

**Maintained by:** Pratham Kumar  
**SRN:** PES2UG24CS368  
**Department:** Computer Science and Engineering  
**PES University**
