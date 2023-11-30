# XOMO/PS

![Constructor Logo](https://github.com/XOMO-PS/XOMO-Repo/raw/main/Images/constructor_logo.png)

**Version:** 2023-11-30

## Changelog

- **2023-11-24:** First draft. Environment requirements added – by Tribe 1-group 3
- **2023-11-25:** First draft. Goals requirements added – by Tribe 1-group 4
- **2023-11-26:** First draft. Project requirements added – by Tribe 1-group 1
- **2023-11-28:** First draft. System requirements added – by Tribe 1-group 2

---

⚠️ _This document follows the requirements book structure presented in the Handbook of requirements and business analysis._

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
- G.1.6. Increasing market demand of the service by making it scalable and flexible

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

- G.4.1 **System users and their details adding functionality:** A user of the system should be able to register on the system.
- G.4.2 **Viewing/accessing available services:** Users of the system or customers should be able to view available services.
- G.4.3 **Searching/filtering masters of services:** Customers should be able to filter best masters of specific service.
- G.4.4 **Ordering/booking services and service payment:** The system should provide service ordering functionality.
- G.4.5 **Feedback giving and rating functionality:** Users of the system should be able to send feedback messages.

### G.5 High-level usage scenarios

XOMO/PS will be hosted on a web server where every user can access using the internet. Operational users will be registered by responsible admins. A new user either as customer (service requesting/providing) registers on the system with his details as needed and be registered user so that he/she can log in to the system as needed. Then the user can view services and requests as per a role on the system orders services and writes feedback.

### G.6 Limitations and exclusions

The system will have the following limitations:

- G.6.1 **Web platform only(will not include mobile version at first deployment):** A mobile version will not be included.
- G.6.2 **No option of choosing users by masters:** The masters will not choose users from the system.

### G.7 Stakeholders and requirements sources

The following stakeholders and requirement sources are identified for the system:

- G.7.1 **Stakeholders:**
  - Project team (Product owner,scum masters, developement team)
  - Operational teams (personnels of system such as customer support and administrators)
  - Customers (service providers and service users)
- G.7.2 **Requirement sources:**
  - Operational teams (people who work on the edn product), customers and literatures

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

#### Job/Work Orders

---

A **Job/Work Order** is a formal request, usually in a documented form, used to authorize and specify the details of maintenance, repair, or other work to be completed. It typically includes information such as the type of job, location, description of tasks, and resources required.

#### Worksheets

---

A **Worksheet** is a document or form used for recording information, planning, and organizing tasks related to a specific job or project. In the context of home services, it often includes details such as client information, service descriptions, time logs, materials used, and any notes relevant to the task at hand. Worksheets are essential for tracking progress, ensuring accountability, and facilitating communication among team members and with clients.

#### Field Services

---

**Field Services** refer to any service performed out in the field, as opposed to at a company property. This encompasses services like repair, maintenance, and installation work typically done at customer homes, business sites, or other external locations.

#### Facility Management

---

**Facility Management** is the practice of coordinating the physical workplace with the people and work of an organization. It integrates principles of business administration, architecture, and the behavioral and engineering sciences to ensure functionality, comfort, safety, and efficiency of the built environment.

#### Site Visits

---

A **Site Visit** involves a professional visiting a location to assess, review, or perform work required. This can be for preliminary assessment, ongoing project management, final inspection, or to provide specific services like repair or maintenance at the site.

#### Tasks

---

A **Task** is an individual unit of work or activity that is a component of a larger project. Tasks are specific, measurable actions with a defined scope and duration. They are the building blocks that, when completed, contribute to the accomplishment of a project's objectives.

#### Projects

---

A **Project** is a larger, overarching endeavor that consists of multiple tasks and activities. It is defined by a set of objectives, a start and end date, and often involves various resources, planning, and coordination. A project is completed when its goals and objectives are achieved, which typically involves the completion of numerous interrelated tasks.

#### Quotations

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
   - The Required Technology Elements are found under "Required Technology Elements" in the [Project Requirements](#project) section of this document.

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

## System Requirements

### Main use cases

**UC1**: As a user, I want to access a list of available services, so as to see which services are offered.

**UC2**: As a user, I want to see a complete list of available masters for existing services, so as to have a choice.

**UC3**: As a customer, I want to be able to order a master for a specific service, so my issue is fixed.

**UC4**: As a master, I want to be able to add myself to the list of masters for specific services, so as to have more clients.

### S1. Components

As we see from the use cases above, we will have these main components:

Frontend (UI) for users and masters to interact with.

Backend for handling requests from frontend and interacting with a database.

Database to keep information about:

- Registered masters.
- Transactions.
- Services.
- Feedbacks.
- Ratings.
- etc.

Infrastructure where everything will run.

### S.2 Functionality

#### S.2.1 **UC1** As a user, I want to access a list of available services, so as to see which services are offered:

- System should show a list of available services.
- System should allow searching/filtering if a list of services is too big (more than 15 services).

#### S.2.2 **UC2** As a user, I want to see a complete list of available masters for existing services, so as to have a choice:

- System should filter out and show available masters for chosen service.
- Short info and rating should be shown for each master.

#### S.2.3 **UC3** As a customer, I want to be able to order a master for a specific service, so my issue is fixed:

- System should show available times of each master on the list of masters.
- System should allow booking a master from the list of masters.
- System should ask for customer information before booking.

#### S.2.4 **UC4** As a master, I want to be able to add myself to the list of masters for specific services, so as to have more clients:

- System should provide a registration form for new masters.
- System should provide a verification process for new masters.

#### S.2.5 Non-functional requirements:

- System should be [_highly available_](https://en.wikipedia.org/wiki/High_availability) (99.9% uptime).
- System should be able to handle ~0.1 qps on average.
- System should be able to serve requests in 3 seconds maximum for 95th percentile of requests.
- System should be able to store 1MB of data.
- System should follow security & privacy best practices for users’ private information.
- System’s UI should be intuitive, which works as the user expects and follows best UI/UX practices.

### S.3 Interfaces

The system’s User Interface should be available via all modern web browsers. The system should adapt to different display sizes, from small phones to big monitors. UI should be intuitive on both Desktop and Mobile interfaces.

The system’s main communication protocol is HTTPS.

### S.4 Detailed Usage Scenarios

#### S.4.1 As a user, I want to specify contact details when ordering a master, so a master can arrive at the place of my choice

- By default, the system should show the most recent contact details of a guest user or profile contact details of a registered user.
- The user should be able to change the contact details:
  - Name
  - Phone number
  - Address:
    - Country (mandatory)
    - State / Region
    - City / Town (mandatory)
    - Street (mandatory)
    - House number (mandatory)
    - Floor
    - Apartment number / name of owner (mandatory)

#### S.4.2 As a user, I want to be able to register on the service, so that my contact details / order history / payment methods are saved

- The form should be shown to a user to enter basic information.
- The provided information should be verified by the system.

#### S.4.3 As a user, I want to be able to login on the service, so that I can re-use my saved information

- The form should be shown to a user to login details:
  - Email
  - Password
- The system should verify the provided information and authorise the user.

#### S.4.4 As a user, I want to view detailed information about masters, so that I can make a better choice of a master

- The system should show a master page with detailed view containing:
  - Master’s name
  - Master’s experience
  - "About" section
  - Provided services
  - Feedbacks from other users
  - Rating
  - etc.

#### S.4.5 As a customer, I want to be able to contact customer service, so that I can ask questions or provide feedback:

- The system should provide contact details of the customer service in visible spots:
  - Email
  - Phone numbers

### S.5 Prioritization

Priority will be measured in 0-4 scale, where:

- 0 - Urgent, critical functionality, the service is unusable without it:
  - S.2.1 As a user, I want to access a list of available services, so as to see which services are offered.
  - S.2.2 As a user, I want to see a complete list of available masters for existing services, so as to have a choice.
  - S.2.3 As a customer, I want to be able to order a master for a specific service, so my issue is fixed.
  - S.4.1 As a user, I want to specify contact details when ordering a master, so a master can arrive at the place of my choice.
- 1 - Required functionality, the service would be in noticeably worse condition for a large user base without it.
  - S.4.5 As a customer, I want to be able to contact customer service, so that I can ask questions or provide feedback.
  - S.2.4 As a master, I want to be able to add myself to the list of masters for specific services, so as to have more clients.
- 2 - Basic functionality which would help most users.
  - S.4.2 As a user, I want to be able to register on the service, so that my contact details / order history / payment methods are saved.
  - S.4.4 As a user, I want to view detailed information about masters, so that I can make a better choice of a master.
  - S.4.3 As a user, I want to be able to login on the service, so that I can re-use my saved information.
- 3 - Optional functionality which is nice to have.
  - As a user, I want to order closest master, so as to fix an urgent issue ASAP.
- 4 - Small functionality which may or may not improve usability of the service.

### S6. Verification & Acceptance Criteria

All P0 and P1 tasks from the previous section should be completed, tested and reviewed by stakeholders.

The UI should work on most modern browsers and display sizes available on the market.

The system should follow non-functional requirements stated in S2.

The system should be accessible globally.

### Optional use cases to consider

#### As a user, I want to order closest master, so as to fix an urgent issue ASAP

- The system should provide an option to find the master for chosen service and closest to the user’s specified location in a couple of clicks.
- The master will be chosen randomly from the list of available masters for the chosen service.
- The location should be taken from the user’s saved address by default.
- The system should find a master in ~2 minutes on average.

---

## Project

The Project book describes all the constraints and expectations not about the system itself but about how to develop and produce it.

### P.1 Roles and personnel

- Requirements Engineer(s)
  - Faruk Avcı
  - Mostafa Emad
  - Adnan Abu Ramadan
  - Gebrearegay
  - Lamin Jawneh
- Product Owner
  - Neha Fathima
- Scrum Master(s)
  - Delilah Garsamo
  - Faris Ahmed
- Developer(s) - Frontend, Backend, Devops
  - Faruk Avci
  - Rishav Ranjan
  - Gebrearegay
  - Emmilly Immaculate
  - Faris Ahmed
  - Lamin Jawneh
  - Adnan Abu Ramadan
  - Mostafa Emad
  - Betselot Aderaw
  - Neha Fathima
  - Shyngys Zhiyenbek
  - Delilah Garsamo
  - Utku Akıncı
  - Mikhail Savrasov

### P.2 Imposed technical choices

- Web framework
  - Web Accessibility Evaluation tools to ensure adherence to Web Content Accessibility Guidelines
- Hosting and scalability
  - Azure Cloud Platform
- DevOps
  - Terraform as IaC

### P.3 Schedule and milestones

#### Gantt Chart

![Schedule Gantt Chart](https://github.com/XOMO-PS/XOMO-Repo/raw/main/Images/Gantt%20Chart%20Schedule.png)

### P.4 Tasks and deliverables

#### P.4.1 Setup Infrastructure

As a developer, I want to be able to deploy services and host the application, so that we can create the product XOMO.

##### Tasks

- Create and setup account on Azure cloud platform
  - using Terraform build IaC to create new business account on Microsoft Azure.
  - every team member has access to account and resources on Azure.
- Integrate support for compute, to create and deploy new services
  - using Terraform build support for deploying new services to App Service on Azure.
- Integrate API Gateway for the service
  - service exposed to internet must pass through API gateway.
- Integrate Key Vault for managing secrets of services
  - when a service needs, it can store secrets in Key Vault.
- Setup domain for platform
  - create descriptive domain name for the service exposed to internet.

#### P.4.2 Handling Emergency Requests by Requesting Callback.

As a user, I want to be able to request a callback, so that I can get help from available master.

##### Tasks

- Design form for emergency service requests.
  - accepts
    - user name, email, address, phone number, location.
    - problem and impact to assess priority.
  - give a message to user to confirm the requested service.
- Design a backend service to process emergency requests
  - an interface which can accept requests from form in #1.
  - forward request to notification service.
- Design a notification system to alert about emergency requests
  - whenever an emergency service is requested.
    - notify the customer support group.

#### P.4.3 Design and Develop User Registration & Login

As a user, I want to be able to register on the XOMO platform, so that I can book services.

##### Tasks

- Design user registration Form.
  - accepts users full name, email, address, phone number, password.
- Design a backend service to store registered users.
  - store the user data in suitable data store.
- Design user login
  - accepts email and password.
- Design a backend service to validate registered users on sign-in
  - validate user data against the stored data.
  - give a clear message, when validation fails.
  - if not fail, navigate user to the main dashboard.

#### P.4.4 Design and Develop Masters/Service Provider Registration

As a service provider, I want to able to register and login to the platform, so that I can join the team of service providers.

##### Tasks

- Design Registration Form.
  - accepts full name,email-address, residence address, phone number, identification method, qualifications,
  - previous experience.
- Design a Backend service to store registered service providers.
  - Store the customer data.
- Design Backend service to store services provided.
  - Store service provider qualification.
- Design Qualifications assessment Form.
  - accepts qualifications in terms of certifications, previous experience, preferred areas of interest for services.
- Design frontend interface for customer to upload documents for identification.
  - requires at-least one document among passport, other identification document.
- Design a Backend service to verify user with provided identification method and document.
  - connect with necessary 3rd party service to verify customer.

#### P.4.5 Design and Develop Search engine

As a user, I want to search for my issue / request type via search bar and see the available masters for that type so that, I can see the available Masters for that type by looking to their features.

##### Tasks

- Design of the search bar
  - Accepts a string with maximum length 100
- Design webpage to available services
  - Provide list of available service.
  - Provide short intro about the service.
- Design webpage to show selected service by user.
  - Selected service information should be listed.
  - Available Masters should be listed next to each other in the format:
  - Each one has a separate grid and grid needs to include minimal information such as rating and reviews
- When a Master is selected, design webpage to show more information
  - Show Public Profile of the Master.
  - Show available dates for booking.
  - On choosing a date, redirect to Booking webpage.
- Design Backend service for Search engine
  - While taking user input for services, provide suggestions by querying backend to find suitable services.
  - Display suitable types of requests / issues (it can be cleaning, electrician, etc.)
  - If no results found, then show all available services.

#### P.4.6 Design and Develop Profile Management

As a user or customer, I want to modify my profile so that, I can change my personal information such as full name, location, occupation, age, biography, and image.

##### Tasks

- Design of the profile page
  - Include text areas for name and biography of user and master.
  - Optionally include other text areas for location, age, and occupation.
  - User and Master can upload profile image.
  - Need save button to save changes to profile.
- Design backend API to send taken inputs from user to it
  - Send information to backend API by clicking to save button
- Modifying image and other profile information.
  - Design backend API to update image
  - When clicked on top of the image and the new image is selected from local, it needs to be sent to corresponding backend API.
- Design Public Profile page for Masters
  - A Master's public information should be displayed for user, which can include
    - Name, Preferred Language of communication.
    - The year since Master is providing services.
    - Reviews and Ratings.
    - Feedback from previously served users.

#### P.4.7 Design and Develop Notification Service

As a user or customer, I want to be notified about upcoming bookings.

##### Tasks

- Design notification webpage
  - Show upcoming bookings with
    - date, time
    - Master assigned for the service.
    - Option to cancel booking given:
      - cancellation date+time is 24 hours before actual service time.
      - cancellation reason.
      - option to reschedule booking.
- Trigger notification once booking is confirmed
  - A push-notification(if enabled) and email to user with booking information.
  - A push-notification(if enabled) and email to Master with booking information.
- Design consent form for Notification.
  - In profile management, user and Master can enable/disable notifications.
  - Option to choose which notification platform is preferred.
  - Show Legal consent policy before enabling the notifications.

#### P.4.8 Design and Develop service for Booking

As a user, I want to see a "Book Now" button next to the profile of a service provider so that I can easily initiate the booking process.

##### Tasks

- Design a booking webpage
  - Display the rates for each available master.
  - Show available dates for each master
  - Dates derived must be in-sync with dates available for each Master.
  - Allow user pick a date.
- Design review booking dialog
  - Add a "Confirm Booking" button for users to finalize their booking.
- Trigger Notification to Master when a user makes a booking.
  - Include relevant details in the notification, such as the user's name, booked service, and date with time(timezone if applicable).
- Design Booking Cancellation dialog
  - A registered, logged-in user should be able to cancel a booking, given:
    - booking identifier.
    - cancellation reason.
    - cancellation date+time is 24 hours before actual service time.
- Design Re-Schedule booking webpage
  - Under booking management, a user or master should be able to reschedule booking given:
    - reschedule date+time is 8 hours before actual service time.

#### P.4.9 Design and Develop Payment Service

As a user, I want to see a "Proceed to Payment" button after confirming my booking so that I can initiate the payment process

##### Tasks

- Design a payment page to show after confirm booking
  - Display the total price for the booking.
  - Allow the user to input card details, including card number, CVV, and cardholder's name.
- Design review payment dialog/page
  - Show a summary of the booking details, including the total price and card details.
  - Add a "Confirm Payment" button for users to finalize the payment.
- Implement a Backend Payment Processing
  - Develop the functionality to proceed with money transfer form the user's account.
  - Integrate a secure payment gateway for processing payments securely.
  - Enable user Receipt Download
- Design and implement the option for users to view and download a payment receipt for their records.
  - Notify Users of Payment Issues
- Trigger notification to users if there are any issues with the payment process
  - provide detailed information on issue.
  - provide alternate payment options.
  - provide option to repeat payment.

#### P.4.10 Design and Develop Feedback service

As a user, I want to be able to provide a feedback, review and ratings for a service, so that I can share my experience.

##### Tasks

- Design a rating page to show after task is finished
  - Allow users to rate the service using a star system (5 highest, 1 lowest).
  - Provide a text box for users to add comments on the master.
- Implement a restriction to allow users to rate only after payment and task completion.
  - Provide dialog for additional optional Feedback to be added.
- Design review section
  - Display stars for each review .
  - Show comments for each review to provide detailed feedback.
- Implement Rating Mechanism
  - Develop the backend functionality to store and calculate ratings for each master.
  - Implement logic to restrict rating eligibility based on payment and task completion.
- Implement Review Mechanism
  - Develop the backend functionality to store and display user reviews for master.
  - Display Review History for Users
- Design and implement a section for to view users own review history.
- Design and implement a section to view master review history.
- Enable Flagging or Reporting of Review
  - Implement a system for users to flag or report inappropriate reviews.
  - Develop a mechanism for platform administrators to review and take appropriate action

### P.5 Required technology elements

#### P.5.1 Software Libraries

##### P.5.1.1 Frontend Libraries

The Frontend component relies on modern frontend libraries to create a responsive and intuitive user interface. Key libraries include:

- **React.js/Vue.js/Angular:** Choosing one for building the interactive user interface.
- **Redux/Vuex/NgRx:** To manage the state of the frontend application.
- **Bootstrap/Tailwind:** To ensure a consistent and mobile-friendly design.

##### P.5.1.2 Backend Framework

The Backend component utilizes a robust backend framework to handle requests and interact with the database. The chosen frameworks are:

- **Spring (Java) / Express (Node.js) / Django (Python) / Flask (Python):** Choosing one for building scalable and maintainable server-side applications.

##### P.5.1.3 Database Management System

The Database component requires a reliable Database Management System to store and manage various data entities. The selected DBMS are:

- **MySQL / PostgreSQL (Java or Node.js)** / **MongoDB (Node.js or Python):** Choosing one based on the backend technology.

##### P.5.1.4 Security Libraries

To adhere to security best practices, the system will implement the following security libraries:

- **Spring Security (Java) / Helmet.js (Node.js) / Django Security (Python) / Flask-Security (Python):** Choosing one for securing the application.
- **bcrypt:** For secure password hashing and storage.

#### P.5.2 Hardware Devices

##### P.5.2.1 Hosting Infrastructure

The entire system will run on a cloud-based infrastructure. Key components include:

- **Cloud Service Provider:** AWS (Amazon Web Services) / Acronis for its reliability and scalability.
- **Virtual Machines:** To host frontend, backend, and database components separately.

##### P.5.2.2 Server Hardware

The server hardware should meet the following specifications to ensure optimal performance:

- **CPU:** Multi-core processors for handling concurrent requests.
- **RAM:** Adequate memory for efficient data processing.
- **Storage:** SSD for fast read and write operations.

#### P.5.3 Communication Protocols

##### P.5.3.1 HTTPS

The main communication protocol for the system is HTTPS. This ensures secure data transfer between the client and the server.

##### P.5.3.2 Language and Localization (Internationalization (i18n) and Localization (l10n) Library)

For comprehensive language support and content localization, the system will integrate an internationalization and localization library. libraries into consideration are:

- **React-Intl / Vue I18n / Angular i18n:** A JavaScript library for internationalization that provides components and an API for formatting dates, numbers, and strings, along with pluralization.

#### P.5.4 External Services

##### P.5.4.1 Payment Gateway Integration

The system will integrate with a reliable payment gateway service to handle transactions securely. Options under consideration include:

- **Stripe:** Known for its global payment processing capabilities.
- **Local Bank Methods:** Since Stripe is not usable in many countries worldwide.

##### P.5.4.2 Geolocation Service

For location-based functionalities, the system may utilize a geolocation service such as:

- **Google Maps API:** To provide accurate location data for service providers and users.

#### P.5.5 Testing Frameworks

##### P.5.5.1 Frontend Testing

To ensure the robustness of the frontend, the following testing frameworks will be employed:

- **Jest (React) / Mocha (Vue, Angular) / Jasmine (Angular):** For unit testing.
- **Cypress / Protractor (Angular):** For end-to-end testing.

##### P.5.5.2 Backend Testing

For backend testing, the system will rely on:

- **JUnit (Java) / Mocha (Node.js) / pytest (Python):** A versatile testing framework.
- **Mockito (Java) / Chai (Node.js) / pytest-mock (Python):** For mocking and testing application components.

### P.6 Risks and mitigation analysis

#### Risk and Mitigation Table

![Risk Table](https://github.com/XOMO-PS/XOMO-Repo/raw/main/Images/Risk%20Table%20Image.png)

### P.7 Requirements process and report

For requirements elicitation, initially we met with many masters (technicians, plumbers, electricians, and so on) by scheduling and preparing interviews with them. Before passing to the interviews, a common question pool had been prepared to collect answers to the similar questions. Until now, interviews have been finished in 10-15 minutes at most by preparing ourselves beforehand.

Currently, lots of requirements are elicited from many customers, users, and stakeholders. After now, we planned the requirement elicitation in the same way as we have made before. Throughout the process we will put our users & customers in the center and try to meet with them by interview mechanism. We will contact with same people more to observe how they feel about product and also we will contact with different people to enlarge our requirements.

Even though workshops our beneficial in eliciting requirements, we will only go with interviews since we have not enough network yet and team is separated to the world that leads to virtual workshops which is not very effective compared to the face-to-face workshops

---

Approved by:                                                        Signature

Date:
