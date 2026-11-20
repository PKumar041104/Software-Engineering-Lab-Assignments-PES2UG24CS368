# Lab 06 – Code and Branch Coverage Analysis

**Course:** UE24CS341A – Software Engineering  
**Semester:** 5th Semester  
**Academic Year:** 2026–27  
**Student Name:** Pratham Kumar  
**SRN:** PES2UG24CS368  
**PRN:** PES2202400086  
**Section:** F  

---

## 1. Objective

To evaluate the completeness of automated software testing using statement coverage and branch coverage techniques. The experiment involved extending the provided test suite, testing normal and boundary conditions, measuring coverage using automated tools, and achieving greater than 90% code and branch coverage.

## 2. Project Overview

**Marathon Registration Application**

The application implements three primary functionalities:

1. **Entry Fee Calculation:** Calculates race registration fees based on race distance, participant age, early-bird discounts, and T-shirt requirements.
2. **Start-Wave Assignment:** Assigns runners to appropriate start waves based on their best recorded time and race category.
3. **Finisher Status Determination:** Determines whether a runner finishes, does not finish (DNF), or is disqualified (DSQ), based on elapsed time and missed checkpoints.

The application was tested using pytest, while coverage.py was used to measure statement and branch coverage.

## 3. Technologies Used

- Python 3.14.0 – Programming language.
- pytest 9.2.0 – Automated test execution.
- coverage.py 7.17.0 – Statement and branch coverage measurement.
- Git – Version control.
- GitHub – Repository hosting and submission.

## 4. Implementation and Testing

The original Marathon Registration application was analysed, and additional test cases were developed to cover different execution paths.

The work included:

- Understanding the original application logic.
- Extending the starter test suite.
- Creating code-coverage test cases.
- Creating branch-coverage test cases.
- Testing normal inputs and boundary conditions.
- Executing automated tests using pytest.
- Measuring statement and branch coverage using coverage.py.
- Verifying uncovered statements and branches.

## 5. Test Coverage Results

The final execution produced the following results:

| Metric | Achieved Result |
|---|---:|
| Code-coverage test cases passed | 35 |
| Line coverage | 100% |
| Branch-coverage test cases passed | 28 |
| Branch coverage | 100% |
| Missing statements | 0 |
| Missing branches | 0 |
| Partially covered branches | 0 |

Both test suites passed successfully. The achieved coverage exceeded the required target of greater than 90%.

## 6. Coverage Analysis

**Statement Coverage:** Measures whether executable statements in the application have been executed by the test suite.

**Branch Coverage:** Measures whether the possible outcomes of decision points, such as conditional statements, have been exercised.

Achieving 100% line and branch coverage indicates that all measured executable statements and branches in the target application were covered by the executed test suites.

## 7. Evidence and Verification

The external GitHub project contains:

- Original Marathon Registration application.
- Starter test file.
- Additional code-coverage test suite.
- Additional branch-coverage test suite.
- Screenshots showing 100% code coverage.
- Screenshots showing 100% branch coverage.
- Consolidated Lab-06 report.

## 8. Learning Outcomes

- Understanding software testing and quality assurance.
- Understanding statement and branch coverage.
- Designing test cases for normal and boundary conditions.
- Using pytest for automated testing.
- Measuring code coverage using coverage.py.
- Identifying uncovered statements and branches.
- Understanding the relationship between test cases and coverage.
- Maintaining software testing projects using Git and GitHub.

## 9. Source Code and Project Documentation

The complete implementation, test suites, screenshots, and supporting project files are maintained in a shared external GitHub repository.

**GitHub Repository:**

https://github.com/PKumar041104/L6_L7_60_marathon_registration

Refer to the `LAB6` directory inside the repository for the complete Lab-06 implementation.

## 10. Conclusion

Lab-06 provided practical experience in evaluating software test completeness using code and branch coverage analysis. The Marathon Registration application was tested using pytest, and coverage.py was used to measure the effectiveness of the test suites.

The final implementation achieved 100% line coverage and 100% branch coverage, with all 35 code-coverage test cases and 28 branch-coverage test cases passing. The experiment demonstrated the importance of systematic test-case design and coverage measurement in improving software testing quality.

---

**Submitted by:** Pratham Kumar  
**SRN:** PES2UG24CS368  
**Department:** Computer Science and Engineering  
**PES University**
