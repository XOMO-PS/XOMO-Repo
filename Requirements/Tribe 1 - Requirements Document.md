# XOMO/PS

![Constructor Logo](Requirements/Pasted image 20231128135314.png)

**Version:** 2023-11-25

## Changelog

- **2023-11-25:** First draft. Goals requirements added – by Tribe 1-group 4

---

⚠️ *This document follows the requirements book structure presented in the Handbook of requirements and business analysis.*

## Contents

- Goals
    - G.1 Context and overall objectives
    - G.2 Current situation
    - G.3 Expected benefits
    - G.4 Functionality overview
    - G.5 High-level usage scenarios
    - G.6 Limitations and exclusions
    - G.7 Stakeholders and requirements sources
- Environment
    - E.1 Glossary
    - E.2 Components
    - E.3 Constraints
    - E.4 Assumptions
    - E.5 Effects
    - E.6 Invariants
- System
    - S.1 Components
    - S.2 Functionality
    - S.3 Interfaces
    - S.4 Detailed usage scenarios
    - S.5 Prioritization
    - S.6 Verification and acceptance criteria
- Project
    - P.1 Roles and personnel
    - P.2 Imposed technical choices
    - P.3 Schedule and milestones
    - P.4 Tasks and deliverables
    - P.5 Required technology elements
    - P.6 Risks and mitigation analysis
    - P.7 Requirements process and report

---

## Goals

### G.1 Context and overall objectives

It is observable that online services are becoming the most important element of daily activity in society. XOMO/PS is an online system connecting people in need with skilled professionals for quick and efficient home service repair and maintenance. The objective of this work is to analyze, design, and implement a web-based system that provides these services at both individual and organizational levels based on request location and service type. It aims to provide an easy and fast service for individuals based on their needs.

#### Main objectives

- G.1.2.   Connecting service requesting and service providers
- G.1.3.   Providing  quality services
- G.1.4.   Providing easy interface for users of the system
- G.1.5.   Providing fast services for requester

### G.2 Current situation

#### What to address?

- G.2.1     Service requesting and service providing  are in invisible barrier
- G.2.2     Skillful professionals are missing due to shortage of connecting platforms
- G.2.3     Very time consuming in getting available  services
- G.2.4      Nearby service providers and service requesting people are not getting to know one another
- G.2.5     Personalized searching of relevant service is not in use
- Flexible booking mechanism of service request is not addressed

### G.3 Expected benefits

The main expected benefits of the project are listed below:

- G.3.1     Saving time and resources
- G.3.2     provide quality and reliable services
- G.3.3     Minimizing efforts of all types
- G.3.4     Wide range of services
	XOMO offers a diverse range of home repair and maintenance services, catering to a variety of customer needs.
- G.3.5     Safety and Security
	Background checks and verification processes for service providers contribute to the safety and security of customers. The platform acts as a third party interested in protecting both users and professionals

### G.4 Functionality overview

Main functionality of the proposed system are listed below:

- G.4.1     **System users adding functionality:** A user of the system should be able to register on the system.
- G.4.2    **Viewing/accessing available services:** Users of the system or customers should be able to view available services.
- G.4.3    **Searching/filtering masters of services:** Customers should be able to filter best masters of specific service.
- G.4.4    **Ordering/booking services:** The system should provide service ordering functionality.
- G.4.5    **Feedback giving functionality:** Users of the system should be able to send feedback messages.

### G.5 High-level usage scenarios

XOMO/PS will be hosted on a web server where every user can access using the internet. Operational users will be registered by responsible admins. A new user either as customer (service requesting/providing) registers on the system with his details as needed and be registered user. Then the user can view services and requests as per a role on the system orders services and writes feedback.

### G.6 Limitations and exclusions

The system will have the following limitations:

- G.6.1     **Service providing hierarchies:** There will no service providers referring mechanism if one could not solve the problem.
- G.6.2     **No distant service will be provided:** All services at the end are physically delivered except consultations.

### G.7 Stakeholders and requirements sources

The following stakeholders and requirement sources are identified for the system:

- G.7.1     **Stakeholders:**
    - Project team (cross-functional teams)
    - Developers, analysts, managers, requirement engineers
    - Operational teams (personnels of system such as customer support and administrators)
    - Customers (service providers and service users)
- G.7.2     **Requirement sources:**
    - Operational teams, customers, repair and maintenance service centers, home service market centers, and literatures

---
## Environment

The Environment book describes the application domain and external context, physical or virtual (or a mix), in which the system will operate.

### E.1 Glossary

Clear and precise definitions of all the vocabulary specific to the application domain, including technical terms, words from ordinary language used in a special meaning, and acronyms.

### E.2 Components

List of elements of the environment that may affect or be affected by the system and project. Includes other systems to which the system must be interfaced.

### E.3 Constraints

Obligations and limits imposed on the project and system by the environment.

⚠️ This section should not be empty!

### E.4 Assumptions

Properties of the environment that may be assumed with the goal of facilitating the project and simplifying the system.

### E.5 Effects

Elements and properties of the environment that the system will affect.

### E.6 Invariants

Properties of the environment that the system’s operation must preserve.


---
# System Requirements
## Main use cases
**UC1**: As a user, I want to access a list of available services, so as to see which services are offered.

**UC2**: As a user, I want to see a complete list of available masters for existing services, so as to have a choice.

**UC3**: As a customer, I want to be able to order a master for a specific service, so my issue is fixed.

**UC4**: As a master, I want to be able to add myself to the list of masters for specific services, so as to have more clients.
## S1. Components
As we see from the use cases above, we will have these main components:

Frontend (UI) for users and masters to interact with.

Backend for handling requests from frontend and interacting with a database.

Database to keep information about:
* Registered masters.
* Transactions.
* Services.
* Feedbacks.
* Ratings.
* etc.

Infrastructure where everything will run.
## S.2 Functionality
#### S.2.1 **UC1** As a user, I want to access a list of available services, so as to see which services are offered:
* System should show a list of available services.
* System should allow searching/filtering if a list of services is too big (more than 15 services).
#### S.2.2 **UC2** As a user, I want to see a complete list of available masters for existing services, so as to have a choice:
* System should filter out and show available masters for chosen service.
* Short info and rating should be shown for each master.
#### S.2.3 **UC3** As a customer, I want to be able to order a master for a specific service, so my issue is fixed:
* System should show available times of each master on the list of masters.
* System should allow booking a master from the list of masters.
* System should ask for customer information before booking.
#### S.2.4 **UC4** As a master, I want to be able to add myself to the list of masters for specific services, so as to have more clients:
* System should provide a registration form for new masters.
* System should provide a verification process for new masters.
#### S.2.5 Non-functional requirements:
* System should be [*highly available*](https://en.wikipedia.org/wiki/High_availability) (99.9% uptime).
* System should be able to handle ~0.1 qps on average.
* System should be able to serve requests in 3 seconds maximum for 95th percentile of requests.
* System should be able to store 1MB of data.
* System should follow security & privacy best practices for users’ private information.
* System’s UI should be intuitive, which works as the user expects and follows best UI/UX practices.
## S.3 Interfaces
The system’s User Interface should be available via all modern web browsers. The system should adapt to different display sizes, from small phones to big monitors. UI should be intuitive on both Desktop and Mobile interfaces.

The system’s main communication protocol is HTTPS.
## S.4 Detailed Usage Scenarios
#### S.4.1 As a user, I want to specify contact details when ordering a master, so a master can arrive at the place of my choice
* By default, the system should show the most recent contact details of a guest user or profile contact details of a registered user.
* The user should be able to change the contact details:
  * Name
  * Phone number
  * Address:
    * Country (mandatory)
    * State / Region
    * City / Town (mandatory)
    * Street (mandatory)
    * House number (mandatory)
    * Floor
    * Apartment number / name of owner (mandatory)
#### S.4.2 As a user, I want to be able to register on the service, so that my contact details / order history / payment methods are saved
* The form should be shown to a user to enter basic information.
* The provided information should be verified by the system.
#### S.4.3 As a user, I want to be able to login on the service, so that I can re-use my saved information
* The form should be shown to a user to login details:
  * Email
  * Password
* The system should verify the provided information and authorise the user.
#### S.4.4 As a user, I want to view detailed information about masters, so that I can make a better choice of a master
* The system should show a master page with detailed view containing:
  * Master’s name
  * Master’s experience
  * "About" section
  * Provided services
  * Feedbacks from other users
  * Rating
  * etc.
#### S.4.5 As a customer, I want to be able to contact customer service, so that I can ask questions or provide feedback:
* The system should provide contact details of the customer service in visible spots:
  * Email
  * Phone numbers
## S.5 Prioritization
Priority will be measured in 0-4 scale, where:
* 0 - Urgent, critical functionality, the service is unusable without it:
  * S.2.1 As a user, I want to access a list of available services, so as to see which services are offered.
  * S.2.2 As a user, I want to see a complete list of available masters for existing services, so as to have a choice.
  * S.2.3 As a customer, I want to be able to order a master for a specific service, so my issue is fixed.
  * S.4.1 As a user, I want to specify contact details when ordering a master, so a master can arrive at the place of my choice.
* 1 - Required functionality, the service would be in noticeably worse condition for a large user base without it.
  * S.4.5 As a customer, I want to be able to contact customer service, so that I can ask questions or provide feedback.
  * S.2.4 As a master, I want to be able to add myself to the list of masters for specific services, so as to have more clients.
* 2 - Basic functionality which would help most users.
  * S.4.2 As a user, I want to be able to register on the service, so that my contact details / order history / payment methods are saved.
  * S.4.4 As a user, I want to view detailed information about masters, so that I can make a better choice of a master.
  * S.4.3 As a user, I want to be able to login on the service, so that I can re-use my saved information.
* 3 - Optional functionality which is nice to have.
  * As a user, I want to order closest master, so as to fix an urgent issue ASAP.
* 4 - Small functionality which may or may not improve usability of the service.
## S6. Verification & Acceptance Criteria
All P0 and P1 tasks from the previous section should be completed, tested and reviewed by stakeholders.

The UI should work on most modern browsers and display sizes available on the market.

The system should follow non-functional requirements stated in S2.

The system should be accessible globally.
## Optional use cases to consider
#### As a user, I want to order closest master, so as to fix an urgent issue ASAP
* The system should provide an option to find the master for chosen service and closest to the user’s specified location in a couple of clicks.
* The master will be chosen randomly from the list of available masters for the chosen service.
* The location should be taken from the user’s saved address by default.
* The system should find a master in ~2 minutes on average.

---
## Project

The Project book describes all the constraints and expectations not about the system itself but about how to develop and produce it.

### P.1 Roles and personnel

Main responsibilities in the project; required project staff and their needed qualifications.

### P.2 Imposed technical choices

Any a priori choices binding the project to specific tools, hardware, languages, or other technical parameters.

### P.3 Schedule and milestones

List of tasks to be carried out and their scheduling.

### P.4 Tasks and deliverables

Details of individual tasks listed under P.3 and their expected outcomes.

### P.5 Required technology elements

External systems, hardware, and software expected to be necessary for building the system.

### P.6 Risks and mitigation analysis

Potential obstacles to meeting the schedule of P.4 and measures for adapting the plan if they do arise.

### P.7 Requirements process and report

Initially description of what the requirements process will be; later report on its steps.



---

Approved by:                                                        Signature

Date:
