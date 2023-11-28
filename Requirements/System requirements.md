# System Requirements
#### Tribe 1 Group 2
#### Status: reviewed
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
