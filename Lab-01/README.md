# Lab 01 – Requirements Engineering & UML Use-Case Modelling

**Course:** UE24CS341A – Software Engineering  
**Semester:** 5th Semester  
**Academic Year:** 2026–27  
**Student Name:** Pratham Kumar  
**SRN:** PES2UG24CS368  
**Date of Experiment:** 19 August 2026

---

## 1. Objective

To elicit and document functional and non-functional requirements from an instructor-provided problem scenario, define measurable acceptance criteria, identify system actors and use cases, and represent the system behaviour using a UML Use-Case Diagram and a detailed Use-Case Flow Specification.

## 2. Problem Statement

**Podcast Guest Scheduling & Outline Builder**

The objective is to design a media production system that simplifies the organization of podcast interviews. The system allows podcast hosts to publish their interview availability, enables guests to book suitable interview slots, collects structured discussion topics and biography links, and generates timestamped run-of-show episode production notes.

The system focuses on simplifying podcast scheduling and improving episode preparation through structured information management.

## 3. Identified Actors

Three primary actors were identified:

1. **Podcast Guest:** Views available interview slots, books a suitable time slot, and submits guest details, biography links and discussion topics.
2. **Show Host:** Creates, updates and blocks interview availability and generates the run-of-show episode outline.
3. **Calendar Service:** Supports the generation and sending of calendar invitations after successful interview bookings.

## 4. Functional Requirements

A total of five Functional Requirements (FR-001 to FR-005) were identified:

| Requirement ID | Description |
|---|---|
| FR-001 | Allows podcast guests to select and book available interview time slots. |
| FR-002 | Allows the Show Host to create, update and block interview time slots. |
| FR-003 | Allows guests to submit structured discussion points and biography links. |
| FR-004 | Sends calendar invitations after successful interview bookings. |
| FR-005 | Generates structured run-of-show episode outlines using guest information and discussion topics. |

## 5. Non-Functional Requirements

Two Non-Functional Requirements were defined:

- **NFR-001 – Performance:** The system must generate the formatted PDF production sheet in under one second.
- **NFR-002 – Security:** Host-specific scheduling and episode-management functions must be restricted to authorized users.

Each requirement was documented with its priority, acceptance criteria and rationale to ensure clarity and testability.

## 6. UML Use-Case Modelling

The UML Use-Case Diagram represents the interactions between the system and its three identified actors.

The following major use cases were modelled:

- Manage Interview Availability
- View Available Slots
- Book Interview Slot
- Submit Guest Details & Discussion Topics
- Send Calendar Invitation
- Generate Run-of-Show Outline

The diagram includes the following relationships:

- **«include»:** Book Interview Slot includes View Available Slots.
- **«extend»:** Send Calendar Invitation extends Book Interview Slot after successful booking.

The diagram illustrates the system boundary, actors, use cases, associations and relationships.

## 7. Use-Case Flow Specification

A detailed use-case flow was prepared for:

**Use Case ID:** UC-02  
**Use Case Name:** Book Interview Slot  
**Primary Actor:** Podcast Guest  
**Supporting Actor:** Calendar Service

The specification contains:

- Preconditions
- Postconditions
- Main Success Scenario
- Alternate Flow – Selected Slot Unavailable

The main success scenario covers selecting an available interview slot, validating availability, confirming the booking, reserving the slot, generating a booking confirmation and sending a calendar invitation.

The alternate flow handles situations where a selected interview slot has already been booked or blocked by the Show Host.

## 8. Learning Outcomes

Through this lab, the following concepts were applied:

- Requirements elicitation and documentation.
- Identification and classification of Functional and Non-Functional Requirements.
- Defining priorities and measurable acceptance criteria.
- Identifying actors and system use cases.
- UML Use-Case Diagram construction.
- Understanding «include» and «extend» relationships.
- Preparing Main Success Scenarios and Alternate Flows.
- Translating a real-world problem scenario into structured software requirements.

## 9. Files Included

| File | Description |
|---|---|
| `PES2UG24CS368-PRATHAM_KUMAR-LAB_1.pdf` | Completed Lab-01 assignment report containing the requirements table, UML explanation and use-case flow. |
| `60_SE_Lab1_SE_Problem_Statements.pdf` | Instructor-provided problem statement for the Podcast Guest Scheduling & Outline Builder. |
| `Student_guidelines` | Lab handout containing objectives, learning outcomes, instructions and deliverables. |

## 10. Conclusion

Lab-01 provided practical experience in Requirements Engineering and UML Use-Case Modelling. The Podcast Guest Scheduling & Outline Builder scenario was analysed to identify its functional and non-functional requirements, actors and use cases. A UML Use-Case Diagram and a detailed use-case flow were prepared to represent the system's functionality and interactions. This exercise demonstrated how an initial problem statement can be transformed into a structured software requirements specification and behavioural model.

---

**Submitted by:** Pratham Kumar  
**SRN:** PES2UG24CS368  
**Department:** Computer Science and Engineering  
**PES University**
