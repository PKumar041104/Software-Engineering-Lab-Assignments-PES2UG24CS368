# Lab 04 – Number Guessing Game Repair

**Course:** UE24CS341A – Software Engineering  
**Semester:** 5th Semester  
**Academic Year:** 2026–27  
**Student Name:** Pratham Kumar  
**SRN:** PES2UG24CS368

---

## 1. Overview

This lab focuses on debugging, repairing, and enhancing an existing Python-based Number Guessing Game using Pygame.

The assignment involved analysing an existing application, identifying its input-handling bug, implementing additional gameplay features, and improving the overall user experience.

The complete implementation and source code are maintained in a separate GitHub repository.

## 2. Project Description

**Number Guessing Game – Pygame Edition**

The application is an interactive number deduction game in which the player attempts to identify a randomly generated secret number between 1 and 100.

The original application provided basic guessing functionality, but contained a deliberate empty-input crash bug and required additional features to improve gameplay.

## 3. Tasks Implemented

The following four tasks were completed:

### Task 1 – Empty Input Crash Fix

- Identified the application crash caused by submitting an empty input.
- Added input validation before integer conversion.
- Displayed a warning message when the input field is empty.
- Ensured that an invalid empty submission does not consume an attempt.

### Task 2 – Dynamic Search Range Display

- Introduced minimum and maximum search boundaries.
- Updated the valid search range after every incorrect guess.
- Displayed the narrowed search range to guide the player.

### Task 3 – Recent Guess History Tracker

- Implemented a guess history panel.
- Displayed the five most recent guesses.
- Added colour-coded indicators for TOO HIGH, TOO LOW, and CORRECT results.

### Task 4 – Maximum Attempts Constraint & Failure State

- Introduced a maximum limit of 10 attempts.
- Implemented a Game Over state when all attempts are exhausted.
- Revealed the secret number after the player loses.
- Added the option to restart the game using the R key.

## 4. Technologies Used

- **Programming Language:** Python
- **Game Development Library:** Pygame
- **Development Concepts:** Input Validation, Exception Prevention, State Management, Conditional Logic, and Object-Oriented Programming.

## 5. Project Structure

The separate GitHub repository contains the following main components:

- `main.py` – Application entry point and main game loop.
- `game/game_engine.py` – Core game logic, attempt tracking, search range management, guess history, and game states.
- `game/text_box.py` – Custom input component for accepting player guesses.
- `README.md` – Project documentation and setup instructions.

## 6. Execution

The application can be executed by following these steps:

1. Clone the project repository.
2. Install Python 3.10 or later.
3. Install the required Pygame dependency.
4. Run the application using:

```bash
pip install pygame
python main.py
```

## 7. Source Code and Implementation

The complete source code, implementation details, project structure, and supporting documentation are available in the separate GitHub repository.

**GitHub Repository:**  
https://github.com/PKumar041104/60_number_guess

Please refer to the linked repository for the complete Lab-04 implementation.

## 8. Learning Outcomes

- Understanding debugging and software repair.
- Identifying and fixing input-handling bugs.
- Implementing input validation.
- Managing dynamic search boundaries.
- Maintaining and displaying recent user activity.
- Implementing attempt limits and game states.
- Working with Python and Pygame.
- Understanding modular programming and object-oriented design.
- Using GitHub for source-code management and project submission.

## 9. Conclusion

Lab-04 provided practical experience in debugging and enhancing an existing Python application. The original Number Guessing Game was improved through empty-input validation, dynamic search range display, recent guess history tracking, and a maximum attempt constraint with a Game Over state.

The complete implementation is maintained in a separate GitHub repository, which is linked in this folder for reference and evaluation.

---

**Submitted by:** Pratham Kumar  
**SRN:** PES2UG24CS368  
**Department:** Computer Science and Engineering  
**PES University
