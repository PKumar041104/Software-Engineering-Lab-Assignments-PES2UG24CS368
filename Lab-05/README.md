# Lab 05 – Static Code Analysis: Student Attendance Tracker

**Course:** UE24CS341A – Software Engineering  
**Semester:** 5th Semester  
**Academic Year:** 2026–27  
**Student Name:** Pratham Kumar  
**SRN:** PES2UG24CS368  
**Section:** F  
**Date of Experiment:** 14 October 2026

---

## 1. Objective

To analyse and improve the quality, security, reliability, and maintainability of an existing Python application using static code analysis tools such as Pylint, Bandit, and Flake8.

The experiment involved identifying issues in the original application, documenting their severity and corrective approaches, implementing fixes, and performing final verification using all three tools.

## 2. Project Overview

**Student Attendance Tracker – Python Application**

The application manages student attendance records and provides functionality for:

- Adding student details.
- Marking daily attendance.
- Calculating attendance percentages.
- Applying the 75% examination eligibility rule.
- Generating attendance shortage lists.
- Detecting consecutive absences.
- Retrieving the latest attendance date.
- Exporting attendance data to CSV.
- Configuring reminder jobs.
- Supporting ERP attendance synchronization.

The original implementation was analysed to identify security vulnerabilities, functional errors, reliability problems, data-integrity issues, and coding-standard violations.

## 3. Technologies and Tools Used

### 3.1 Pylint – Code Quality Analysis

Pylint was used to identify:
- Missing module and function documentation.
- Incorrect naming conventions.
- Unused imports and variables.
- Mutable default arguments.
- Unnecessary Boolean comparisons.
- Code-quality and maintainability issues.

### 3.2 Bandit – Security Analysis

Bandit was used to identify potential security vulnerabilities, including:
- Disabled TLS certificate verification.
- Unsafe shell-based command execution.
- Wildcard injection risks.
- Outdated TLS configuration.
- HTTP requests without timeouts.

### 3.3 Flake8 – Coding Standard Analysis

Flake8 was used to identify:
- PEP 8 violations.
- Incorrect indentation and spacing.
- Unused imports.
- Excessive line lengths.
- Formatting inconsistencies.
- Unnecessary comparisons.

## 4. Initial Baseline Analysis

The original Attendance Tracker application was executed and analysed before making modifications.

The initial results were:

| Tool | Initial Result |
|---|---|
| Pylint | 4.55/10 |
| Bandit | 8 findings (2 High, 3 Medium, 3 Low) |
| Flake8 | Multiple coding-style violations |

These results established the baseline quality and security condition of the original application.

## 5. Issues Identified and Corrective Actions

The original application was reviewed for security, functional correctness, reliability, data integrity, and maintainability issues.

The major issues and their corrective approaches included:

| Issue | Corrective Action |
|---|---|
| Disabled TLS certificate verification | Restored default TLS certificate verification. |
| Shell-based archive creation | Replaced shell commands with Python's `tarfile` module. |
| Hard-coded API-key configuration | Used an environment variable for API-key retrieval. |
| Outdated TLS protocol | Replaced the legacy configuration with a secure default SSL context. |
| Missing HTTP timeout | Added a 10-second request timeout and response-status validation. |
| Mutable default argument | Changed the default argument to `None` and initialized it safely. |
| Incorrect 75% eligibility boundary | Used an inclusive `>=` comparison. |
| Division-by-zero risk | Added handling for students with no attendance records. |
| Duplicate attendance records | Added duplicate-entry prevention. |
| Inconsistent date formats | Implemented ISO-format date validation and normalization. |
| CSV formula injection | Added protection for formula-leading text values during export. |
| Code-quality violations | Improved naming, documentation, resource handling, encoding, and formatting. |

Detailed issue descriptions, original source references, classifications, and fix approaches are maintained in the external project's `issues.md` file.

## 6. Code Correction and Implementation

The original Attendance Tracker application was modified to address the identified issues.

The corrected implementation included:

- Secure HTTP communication with certificate verification.
- Environment-based API-key configuration.
- Safe archive creation without shell execution.
- HTTP timeout and response-status handling.
- Safe attendance percentage calculation.
- Inclusive attendance eligibility evaluation.
- Duplicate attendance prevention.
- Validated and normalized attendance dates.
- Safer CSV export.
- Improved resource management and code documentation.

The corrected application was maintained as a modular Python implementation in `attendance_tracker.py`.

## 7. Final Static Analysis Results

After implementing the corrections, all three static analysis tools were executed again.

| Tool | Final Result | Interpretation |
|---|---|---|
| Pylint | 10.00/10 | Perfect code-quality score. |
| Bandit | 0 findings | No issues identified by the final scan. |
| Flake8 | 0 violations | No reported coding-style violations. |

The final results demonstrated significant improvement compared with the initial baseline.

## 8. Functional Execution Verification

The corrected application was executed locally to verify its functionality.

The offline demonstration covered:

- Attendance percentage calculation.
- Verification of the 75% eligibility condition.
- Generation of attendance shortage lists.
- Detection of consecutive absences.
- Retrieval of the latest attendance date.
- Date-wise attendance registration.
- CSV attendance export.
- Reminder-job configuration.

The ERP synchronization operation was intentionally skipped during the offline demonstration because it requires an appropriate API key and a reachable ERP endpoint.

## 9. Evidence and Verification

The external project contains the following supporting evidence:

- Fresh repository clone.
- Baseline execution of the original application.
- Initial Pylint analysis.
- Initial Bandit security analysis.
- Initial Flake8 analysis.
- Final verification using all three tools.
- Before-and-after text reports for each analysis tool.

These records provide evidence of the analysis process and the improvements achieved after applying the corrections.

## 10. Reflection and Learning Outcomes

The experiment provided practical understanding of:

- Static code analysis and its importance in software development.
- Identifying programming errors without relying only on execution.
- Detecting common security vulnerabilities.
- Improving Python code quality and maintainability.
- Applying Pylint, Bandit, and Flake8.
- Fixing functional boundary-condition errors.
- Understanding secure HTTP communication.
- Implementing input validation and data-integrity checks.
- Comparing baseline and final analysis results.
- Understanding why multiple analysis tools are required for comprehensive code review.

An important learning outcome was that different static analysis tools identify different categories of problems. No single tool guarantees complete software correctness or security. Their results should be considered alongside functional testing and manual code review.

## 11. Source Code and Project Documentation

The complete implementation, source code, issue analysis, reflection responses, screenshots, and before-and-after analysis reports are maintained in a separate GitHub repository.

**External GitHub Repository:**

https://github.com/PKumar041104/L5_61_attendance-tracker

Refer to this repository for the complete Lab-05 implementation and supporting evidence.

## 12. Conclusion

Lab-05 provided practical experience in improving Python application quality through static code analysis. The Student Attendance Tracker was analysed using Pylint, Bandit, and Flake8. Security vulnerabilities, functional errors, reliability problems, data-integrity issues, and coding-standard violations were identified and corrected.

Following the corrections, the application achieved a Pylint score of 10.00/10, Bandit reported no identified issues, and Flake8 reported no violations. The corrected application also completed its recorded offline functional demonstration.

The experiment demonstrated the importance of iterative code analysis, secure programming practices, and verification in developing reliable and maintainable software.

---

**Submitted by:** Pratham Kumar  
**SRN:** PES2UG24CS368  
**Department:** Computer Science and Engineering  
**PES University**
