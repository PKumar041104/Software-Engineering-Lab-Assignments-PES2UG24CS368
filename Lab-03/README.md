# Lab 03 – Component Modelling & Architectural Pattern Selection

**Course:** UE24CS341A – Software Engineering  
**Semester:** 5th Semester  
**Academic Year:** 2026–27  
**Student Name:** Pratham Kumar  
**SRN:** PES2UG24CS368  
**PRN:** PES2202400086  
**Section:** F  
**Date of Experiment:** 09 September 2026

---

## 1. Objective

To evaluate different software architectural styles, select the most appropriate architecture for the assigned problem scenario, and understand component modelling, UML Component Diagrams, interfaces, and dependencies.

## 2. Project Scenario

**Podcast Guest Scheduling & Outline Builder**

This lab continues the project scenario introduced in Lab-01 and Lab-02.

The system supports podcast interview scheduling, host availability management, guest information collection, calendar integration, and generation of structured episode production outlines.

The objective of this experiment was to identify a suitable software architecture that provides clear separation of responsibilities, maintainability, security, and efficient processing.

## 3. Architectural Styles Analysed

Three architectural styles were studied and evaluated:

### 3.1 Layered Architecture

Organizes the application into horizontal layers, such as Presentation, Business, and Data.

**Advantages:**
- Clear separation of concerns.
- Easy to understand and maintain.
- Suitable for traditional applications.

**Limitations:**
- Performance overhead between layers.
- Potential tight coupling between layers.
- Difficult to scale individual components independently.

### 3.2 Microservices Architecture

Organizes the application into small, independently deployable services.

**Advantages:**
- Independent scaling.
- Fault isolation.
- Technology diversity.
- Independent deployment.

**Limitations:**
- Operational complexity.
- Network latency.
- Data consistency challenges.

### 3.3 Client-Server Architecture

Uses a centralized server to provide services to multiple clients.

**Advantages:**
- Centralized control.
- Simple deployment.
- Easier data consistency.

**Limitations:**
- Single point of failure.
- Scalability bottleneck.
- Limited fault tolerance.

## 4. Selected Architecture

**Selected Architecture: Layered Architecture**

Layered Architecture was selected for the Podcast Guest Scheduling & Outline Builder because it provides a clear separation between the user interface, application logic, and data management.

The system is organized into three logical layers:

1. **Presentation Layer:** Handles interactions with the Podcast Guest and Show Host.
2. **Business Layer:** Handles interview scheduling, guest information management, and episode outline generation.
3. **Data Layer:** Manages persistent podcast data.

This architecture provides the required organization without introducing the additional operational complexity of independently deployed microservices.

## 5. Architectural Justification

The selection was supported by the following considerations:

### Clear Separation of Responsibilities

Different system functions are assigned to appropriate layers, making the application easier to understand, develop, and maintain.

### Suitability for System Scope

The system contains a focused set of related functionalities. A layered structure provides sufficient modularity without requiring independently deployable services for every function.

### Security Advantage

Authorization checks can be handled before host-specific operations reach the data layer. This helps restrict interview availability management and episode-management functions to authorized users.

This supports **NFR-002**, which requires host-specific scheduling and episode-management functions to be accessible only to authorized users.

### Performance Benefit

The layered structure keeps the main application processing within the system and avoids unnecessary network communication between independently deployed microservices.

This can help reduce communication overhead during production-sheet generation and supports **NFR-001**, which requires the formatted PDF production sheet to be generated in under one second.

## 6. UML Component Modelling Concepts

The lab handout covered the following UML Component Diagram concepts:

- Component notation using the `<<component>>` stereotype.
- Provided interfaces represented using ball notation.
- Required interfaces represented using socket notation.
- Ports as component interaction points.
- Usage dependencies represented using dashed arrows with the `<<use>>` stereotype.
- Assembly connectors between provided and required interfaces.

The assignment required a component diagram containing at least five components and at least four interfaces, showing component interactions and data flow.

## 7. Learning Outcomes

- Understanding different software architectural styles.
- Comparing Layered, Microservices, and Client-Server architectures.
- Selecting an appropriate architecture based on system requirements.
- Understanding modular software components.
- Learning UML Component Diagram notation.
- Understanding provided and required interfaces.
- Identifying component dependencies and interactions.
- Analysing security and performance implications of architectural decisions.
- Documenting and justifying architectural choices.

## 8. Files Included

| File | Description |
|---|---|
| `Lab_3_Architecture_Student_handout (1).pdf` | Instructor-provided lab instructions, architectural concepts, scenario, and deliverables. |
| `PES2UG24CS368_PRATHAM-KUMAR_Lab3-UML_Component_Diagram.pdf` | Completed assignment report containing the selected architecture and detailed justification. |

## 9. Conclusion

Lab-03 provided practical understanding of software architectural styles and component modelling. Layered Architecture was selected for the Podcast Guest Scheduling & Outline Builder because it offers clear separation of responsibilities, suits the system scope, supports controlled access to host-specific operations, and helps reduce unnecessary communication overhead. The experiment strengthened understanding of architectural selection, UML component concepts, security considerations, and performance implications in software design.

---

**Submitted by:** Pratham Kumar  
**SRN:** PES2UG24CS368  
**Department:** Computer Science and Engineering  
**PES University**
