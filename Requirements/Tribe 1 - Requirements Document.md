# XOMO/PS

![Constructor Logo](Pasted image 20231128135314.png)

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

### Environment User Stories

1. **For Service Providers and Users (E2: Components)**
   - As a service provider, I want to efficiently list and manage my services on the platform, and as a user, I want to easily find, book, and pay for these services, so that both parties can benefit from a streamlined and secure transaction process.


2. **For Platform Functionality and User Experience (E3: Constraints, E4: Assumptions)**
   - As a platform designer, I want to create a system that is technologically compatible, easy to navigate, and performs well under varying internet connectivity conditions, assuming users have basic technological proficiency and device accessibility, so that we can provide a seamless and inclusive experience for all users.


3. **For Regulatory Compliance and Payment Processing (E3: Constraints, E6: Invariants)**
   - As a platform administrator, I want to ensure that the platform adheres to all relevant laws and regulations, including data privacy, and offers a stable and reliable payment gateway, so that we can maintain legal compliance and user trust while ensuring smooth financial transactions.


4. **For Scalability and Market Demand (E3: Constraints, E4: Assumptions)**
   - As a business strategist, I want the platform to be scalable and flexible to accommodate a growing number of users and transactions, while assuming there is sustained market demand for our services, so that we can expand our reach and adapt to changing market conditions.


5. **For User Interface and Accessibility (E3: Constraints, E5: Effects)**
   - As a UX/UI designer, I want to develop a user-friendly interface that adapts to different devices and screen sizes, considering users' varied technological capabilities and preferences, so that we can ensure accessibility and a positive experience for every user.


6. **For Service Reliability and Data Accuracy (E3: Constraints, E4: Assumptions, E6: Invariants)**
   - As a service provider, I want to rely on the platform's stability, including its integrations with payment gateways and external APIs, and assume that the data provided by users is accurate, so that I can offer consistent and reliable services to my clients.


7. **For User Engagement and Feedback (E4: Assumptions, E5: Effects)**
   - As a community manager, I assume users will engage positively and responsibly, providing fair ratings and constructive feedback, while adapting to the effects of regulatory changes and internet connectivity fluctuations, so that we can maintain a vibrant and responsive service community.


### E.1 Glossary

#### Facility Services

---
**Facility Services** encompass a wide range of activities essential for the maintenance, care, and management of commercial and residential buildings. This includes services like cleaning, security, HVAC (heating, ventilation, and air conditioning) maintenance, and other tasks that ensure the functionality, safety, and efficiency of a facility.

#### HVAC Services

---
**HVAC Services** refer to the installation, maintenance, and repair of heating, ventilation, and air conditioning systems. This is crucial for maintaining a comfortable and safe indoor environment.

#### Plumbing Services

---
**Plumbing Services** involve the installation, repair, and maintenance of pipes, fixtures, and other apparatuses for the distribution and use of water in a building. It also includes addressing issues like leaks, blockages, and water pressure problems.

#### Electrical Services

---
**Electrical Services** cover the installation, repair, and maintenance of electrical systems, including wiring, outlets, lighting, and power systems in buildings. This also encompasses ensuring safety standards are met to prevent hazards.

#### Landscaping Services

---
**Landscaping Services** include garden design, lawn care, tree planting and maintenance, and the construction of outdoor features like paths and retaining walls. It enhances the aesthetic appeal and functionality of outdoor spaces.

#### Cleaning Services

---
**Cleaning Services** involve the thorough cleaning, sanitizing, and upkeep of different areas within a building, including floors, windows, restrooms, and common areas.

#### Pest Control Services

---
**Pest Control Services** manage and eliminate unwanted pests like insects, rodents, and other animals that can cause damage or health risks in a building.

#### Handyman Services

---
**Handyman Services** encompass a broad range of home repair and maintenance tasks, from fixing leaky faucets to painting walls and assembling furniture.

#### Home Security Services

---
**Home Security Services** include the installation and monitoring of security systems like alarms, cameras, and motion sensors to protect a property from intrusion or damage.

#### Job/Work Order

---
A **Job/Work Order** is a formal request, usually in a documented form, used to authorize and specify the details of maintenance, repair, or other work to be completed. It typically includes information such as the type of job, location, description of tasks, and resources required.

#### Worksheet

---
A **Worksheet** is a document or form used for recording information, planning, and organizing tasks related to a specific job or project. In the context of home services, it often includes details such as client information, service descriptions, time logs, materials used, and any notes relevant to the task at hand. Worksheets are essential for tracking progress, ensuring accountability, and facilitating communication among team members and with clients.

#### Field Services

---
**Field Services** refer to any service performed out in the field, as opposed to at a company property. This encompasses services like repair, maintenance, and installation work typically done at customer homes, business sites, or other external locations.

#### Facility Management

---
**Facility Management** is the practice of coordinating the physical workplace with the people and work of an organization. It integrates principles of business administration, architecture, and the behavioral and engineering sciences to ensure functionality, comfort, safety, and efficiency of the built environment.

#### Site Visit

---
A **Site Visit** involves a professional visiting a location to assess, review, or perform work required. This can be for preliminary assessment, ongoing project management, final inspection, or to provide specific services like repair or maintenance at the site.

#### Task

---
A **Task** is an individual unit of work or activity that is a component of a larger project. Tasks are specific, measurable actions with a defined scope and duration. They are the building blocks that, when completed, contribute to the accomplishment of a project's objectives.

#### Project

---
A **Project** is a larger, overarching endeavor that consists of multiple tasks and activities. It is defined by a set of objectives, a start and end date, and often involves various resources, planning, and coordination. A project is completed when its goals and objectives are achieved, which typically involves the completion of numerous interrelated tasks.

#### Quotation

---
A **Quotation** is a formal statement or document that outlines the estimated cost for products or services. In the context of home services, it usually includes a detailed breakdown of the work to be done, the materials required, labor costs, and any other expenses. Quotations are provided to potential customers before any work begins, allowing them to understand and agree to the pricing and scope of the job.

---
### E.2 Components

1. **Service Providers**
   - **Description:** Businesses or individual professionals who offer home services like plumbing, electrical work, cleaning, etc. They are the primary customers of the platform, using it to list their services, receive job orders, and interact with users.

2. **Users**
   - **Description:** Individuals or organizations that use the platform to find and book home services. They interact with the system to schedule, pay for services, and provide feedback.

3. **Booking System**
   - **Description:** An interface for users to schedule services. Includes functionality for selecting service types, choosing providers, setting dates and times, and specifying job details.

4. **Payment Gateway**
   - **Description:** A secure system for processing payments, handling transactions between users and service providers, including invoicing, payment collection, and financial record-keeping.

5. **User Profiles**
   - **Description:** Accounts for users and service providers, storing information such as personal details, service history, preferences, and ratings.

6. **Rating and Review System**
   - **Description:** Allows users to rate and review the services they receive, which helps maintain quality and trust on the platform.

7. **Notification System**
   - **Description:** Sends alerts and updates to users and service providers, including appointment reminders, service status updates, and other important notifications.

8. **Administrative Dashboard**
   - **Description:** A backend interface for platform administrators to manage users, oversee transactions, and analyze platform performance.

9. **Support System**
   - **Description:** Handles inquiries, complaints, and assistance requests from users and service providers, through channels like chat, email, and phone.

10. **Content Management System (CMS)**
    - **Description:** Manages content on the platform, such as service descriptions & posts, blog posts, FAQs, and other resources.

11. **Analytics and Reporting Tools**
    - **Description:** Tools for analyzing user behavior, service performance, financial transactions, and other key metrics.

12. **Security Features**
    - **Description:** Ensures security and privacy of data, transactions, and interactions on the platform, including encryption, authentication, and data protection.

### E.3 Constraints

1. **Regulatory Compliance**
   - **Description:** The system must adhere to all relevant laws and regulations, including data privacy laws (like GDPR), labor laws, and industry-specific regulations. This can limit how data is collected, stored, and processed.

2. **Technological Compatibility**
   - **Description:** The system should be compatible with various desktop devices and browsers.

3. **Network Connectivity**
   - **Description:** The system's performance is contingent on internet connectivity. In areas with limited or unreliable internet access, functionality might be constrained.

4. **Payment Processing Restrictions**
   - **Description:** Payment gateways may have restrictions on certain types of transactions, currencies, or geographical locations, impacting the ability to process payments globally.

5. **User Interface Limitations**
   - **Description:** The need for a user-friendly interface may limit the complexity of features that can be implemented, balancing advanced functionality with ease of use.

6. **Resource Constraints**
   - **Description:** Budgetary, staffing, and time constraints can affect the scope of features and services that can be developed and maintained. Example: Customer Service Call Centre limitations.

7. **Scalability Limits**
   - **Description:** The system’s ability to scale up to accommodate an increasing number of users and transactions can be limited by current infrastructure and technology.

8. **Language and Localization**
   - **Description:** The system might be limited in offering multilingual support or localizing content for different regions, affecting its usability in diverse markets.

9. **Third-Party Dependencies**
    - **Description:** Reliance on third-party services (like cloud hosting, APIs, etc.) can impose constraints based on their availability, performance, and feature set.
    - This will need to be elaborated on based on P.5 - Required Technology Elements.

### E.4 Assumptions

1. **Stable Internet Access**
   - **Assumption:** Users and service providers have consistent and reliable access to the internet to use the platform effectively.

2. **Technological Proficiency**
   - **Assumption:** Both users and service providers possess a basic level of technological proficiency, enabling them to navigate and utilize the app's features without extensive training.

3. **Device Accessibility**
   - **Assumption:** A significant portion of the user base owns or has access to devices capable of running the web app.

4. **Payment Gateway Reliability**
   - **Assumption:** The integrated payment gateways are reliable and can handle the transaction volume without significant downtime or errors.

5. **Market Demand**
   - **Assumption:** There is a sustained demand for home services offered through online platforms in the target market.

6. **Data Accuracy**
   - **Assumption:** Information provided by users and service providers, such as contact details, service requirements, and availability, is accurate and up-to-date.

7. **Compliance Willingness**
   - **Assumption:** Service providers using the platform will comply with all relevant laws, regulations, and quality standards.

8. **Positive User Behavior**
   - **Assumption:** Users will engage positively and responsibly on the platform, including fair ratings and constructive feedback.

9. **Third-Party Service Stability**
    - **Assumption:** Third-party services and APIs integrated into the platform will remain stable and consistent in their offerings and performance.


### E.5 Effects

1. **Internet Connectivity Fluctuations**
   - **Effect:** Variations in internet speed or connectivity issues can affect the app’s responsiveness and accessibility, potentially leading to a poor user experience or transaction failures.

2. **Device Compatibility Changes**
   - **Effect:** Updates or changes in components, user devices and their operating systems can impact the app's compatibility, requiring frequent updates or adaptations.

3. **Regulatory Changes**
   - **Effect:** New laws or changes in regulations (like privacy laws or labor regulations) can necessitate adjustments in how the platform operates, particularly in data handling and service provider management.

4. **Changing Browser Window Size**
   - **Effect:** When users resize their browser windows, it can affect the display and layout of the web app. This necessitates a responsive design that adapts seamlessly to different screen sizes and orientations, ensuring a consistent and user-friendly experience regardless of the device used.

### E.6 Invariants

1. **Payment Gateway Integration** 
   - **Invariant:** The integration with payment gateways remains stable, ensuring consistent and reliable processing of transactions.

2. **API Integration Stability**
   - **Invariant:** The integration with external APIs, such as mapping services or external databases, remains stable, ensuring seamless interaction and data exchange.


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
