# Lab 07 – Fuzzing for Input Validation Bugs

**Course:** UE24CS341A – Software Engineering  
**Semester:** 5th Semester  
**Academic Year:** 2026–27  
**Student Name:** Pratham Kumar  
**SRN:** PES2UG24CS368  
**PRN:** PES2202400086  
**Section:** F  

---

## 1. Objective

To explore fuzz testing as a software quality assurance technique by identifying and fixing input-validation defects in a Python application using property-based testing with the Hypothesis library.

The experiment involved generating unexpected, malformed, and invalid inputs automatically to identify runtime exceptions and improve application robustness through defensive programming.

## 2. Project Overview

**Marathon Registration Parser**

The application processes marathon registration information through three primary functions:

1. **format_bib_name():** Converts a runner's name into uppercase and limits it to 12 characters for the race bib.
2. **parse_finish_time():** Converts a marathon finish time in H:MM:SS format into its equivalent value in seconds.
3. **average_split():** Calculates the average of space-separated split times provided in minutes.

The original implementation assumed that all inputs would be valid and correctly formatted. Property-based fuzz testing was used to identify input-validation weaknesses.

## 3. Technologies Used

- Python 3.14.0 – Programming language.
- Hypothesis 6.170.15 – Property-based fuzz testing.
- pytest 9.2.0 – Automated test execution.
- Git – Version control.
- GitHub – Repository hosting and submission.

## 4. Fuzz Testing Methodology

Hypothesis was used to automatically generate a wide range of inputs rather than relying only on manually selected test values.

The experiment followed the six steps specified in the laboratory workflow.

### Step 1 – Installing Dependencies

Installed the required Python libraries:

```powershell
python -m pip install hypothesis
python -m pip install pytest
```

### Step 2 – Running the Original Application

Executed the original application:

```powershell
python marathon_registration_parser.py
```

The normal behaviour of the three application functions was checked using valid sample inputs.

### Step 3 – Completing the Hypothesis Test File

Completed the provided test template, `test_marathon_registration_parser.py`.

Implemented three property-based no-crash tests using Hypothesis strategies to generate arbitrary text inputs and None values.

### Step 4 – Testing the Original Application

Executed:

```powershell
python -m pytest test_marathon_registration_parser.py
```

All three test functions initially failed, exposing input-validation defects.

The identified runtime exceptions included:

- AttributeError – Operations performed on None values.
- ValueError – Invalid or malformed inputs during numeric conversion.
- ZeroDivisionError – Attempting to calculate an average from empty input.

**Initial Result: 3 Failed**

### Step 5 – Fixing the Application

Modified `marathon_registration_parser.py` using defensive programming techniques.

The corrections included:

- Input type validation.
- Empty-input validation.
- Input-format verification.
- ASCII digit validation.
- Exception handling for numeric conversions.
- Validation of minute and second ranges.
- Graceful handling of invalid results in the main function.

Invalid inputs are handled safely by returning None, while meaningful error messages are displayed to the user.

### Step 6 – Re-executing Hypothesis Tests

Executed the same test suite against the corrected implementation:

```powershell
python -m pytest test_marathon_registration_parser.py
```

All three test functions passed successfully.

**Final Result: 3 Passed**

## 5. Before-and-After Test Results

| Test Function | Original Application | Corrected Application |
|---|---|---|
| test_format_bib_name_no_crash() | Failed | Passed |
| test_parse_finish_time_no_crash() | Failed | Passed |
| test_average_split_no_crash() | Failed | Passed |
| **Total** | **3 Failed** | **3 Passed** |

The same test suite was used before and after modifying the application to evaluate the effectiveness of the corrections consistently.

## 6. Error Handling and Defensive Programming

The experiment demonstrated the importance of validating user inputs before performing string operations, numeric conversions, and mathematical calculations.

The corrected implementation prevents the identified runtime exceptions for the inputs exercised by the Hypothesis tests and provides safer handling of malformed data.

## 7. Evidence and Verification

The external GitHub project contains:

- Original Marathon Registration Parser application.
- Corrected parser implementation.
- Completed Hypothesis-based test file.
- Original application execution screenshot.
- Dependency installation screenshot.
- Screenshot of failing Hypothesis tests.
- Corrected application execution screenshot.
- Screenshot of passing Hypothesis tests.
- Consolidated Lab-07 report.

## 8. Learning Outcomes

- Understanding fuzz testing.
- Understanding property-based testing.
- Using Hypothesis to generate unexpected inputs.
- Identifying input-validation defects.
- Understanding AttributeError, ValueError, and ZeroDivisionError.
- Applying defensive programming.
- Implementing input type and format validation.
- Testing software behaviour with malformed and unexpected inputs.
- Comparing original and corrected application behaviour.
- Using pytest and Hypothesis together for automated testing.

## 9. Source Code and Project Documentation

The complete implementation, Hypothesis test suite, screenshots, and supporting project files are maintained in the same external GitHub repository used for Lab-06.

**GitHub Repository:**

https://github.com/PKumar041104/L6_L7_60_marathon_registration

Refer to the `LAB7` directory inside the repository for the complete Lab-07 implementation.

## 10. Conclusion

Lab-07 provided practical experience in identifying and correcting input-validation defects through property-based fuzz testing. The original Marathon Registration Parser application was tested using Hypothesis, which generated unexpected inputs and exposed runtime exceptions in all three application functions.

After implementing input validation and defensive programming techniques, all three Hypothesis test functions passed successfully. The experiment demonstrated the importance of testing software with unexpected inputs and improving application robustness through systematic automated testing.

---

**Submitted by:** Pratham Kumar  
**SRN:** PES2UG24CS368  
**Department:** Computer Science and Engineering  
**PES University**
