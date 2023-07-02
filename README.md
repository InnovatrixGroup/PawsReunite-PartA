# PawsReunite

[Click here](https://github.com/InnovatrixGroup/PawsReunite-PartA) to access the GitHub Repository.

## Table of Contents

1. [Description](#description)
2. [Dataflow Diagram](#dataflow-diagram)
3. [Application Architecture Diagram](#application-architecture-diagram)
4. [User Stories](#user-stories)
5. [Wireframes](#wireframes)
6. [Project Planning and Management](#project-planning-and-management)

## Description

### Purpose

According to estimates, one out of every three pets will go missing at some point in their lives. Millions of pets are missing every year, and many of them may never return home.

The purpose of PawsReunite is to help pet owners find their lost pets and to help people who have found lost pets find their owners. This is a valuable service because lost pets can be very difficult to find, and even if they are found, it can be difficult to track down their owners. This web application can help to bridge this gap by providing a central platform where pet owners and people who have found lost pets can connect.

____
### Functionality/ Feature

#### User Registration and Authentication: 
   
To create a lost/found pet post, users must create new accounts first, so they can be contacted when there is any update. 

Comparing to general users, admin users will have the authorisation to remove inappropriate or irrelevant content, such as spam or offensive posts. Admin users can also remove certain users and all related posts.

#### Report lost pet

Pet owners can report their lost pets, providing details such as pet characteristics (including colour, breed and other descriptions), photos, last seen location and contact information.

#### Report found pet

Users who find a lost pet can report it, providing details such as pet description, photos, found location and contact information.

#### Pet Search

Users can search for lost pets based on location, colour, breed, or other characteristics. Based on the provided information, the application will display a list of lost pets that match the search criteria.

#### Communication

To facilitate better communication between the users, users can leave comments under the lost/found pet posts so they can provide helpful information if available.

#### Pet Care Resources

Users are able to find information about pet care on the platform. This information includes articles, tips, and links to other websites.

#### Potential Match and Notification (Nice to have): 

The application runs a matching algorithm to connect lost pets with found pet based on similar characteristics, such as breed, colour, or lost/found location. Users will receive in-app and email notifications when a potential match is found.

____
### Target Audience

The target audience for PawsReunite is pet owners, people who have found lost pets, and animal shelters or rescue organizations. Pet owners are the primary users of this application, as they are the ones who are most likely to be looking for lost pets. People who have found lost pets are also potential users, as they may be looking for a way to reunite the pet with its owner. Animal shelters and rescue organizations can also use this app to help find homes for lost pets.

____
### Tech Stack



## Dataflow Diagram

### User Management

![Dataflow diagram - User Management](./docs/DFD-user%20management.png)

### Lost/Found Pet Post Management

![Dataflow diagram - Lost/Found Pet Post Management](./docs/DFD-pet%20post%20management.png)

### Comment Management

![Dataflow diagram - Comment Management](./docs/DFD-comment%20management.png)

### User Notifications

![Dataflow diagram - User Notifications](./docs/DFD-notification%20management.png)


## Application Architecture Diagram

![Application Architecture Diagram](./docs/Application%20Architecture%20disgram.png)

### Client Side

Our web application is built with compatibility in mind, ensuring it can be accessed by a wide range of modern browsers. Whether you prefer Chrome, Firefox, Safari, Edge, or any other popular browser, you can rest assured that our application is designed to work smoothly and efficiently on each of them. 
___
### Frontend User Interface Layer
Frontend Components: This layer includes the user interface components that users interact with, such as web pages, forms, search interfaces.

____
### Backend Application Layer
1. Web Server: The web server handles incoming requests from clients and routes them to the appropriate backend components.

2. Application Logic: This layer contains the core logic of the application, including handling lost and found pet postings, search functionality, and interactions with the database.

3. API Gateway: Acts as a single entry point for clients to access backend services and manages API requests and responses.

___
### Services and Integration Layer

1. Database: Stores and manages data related to lost and found pet postings, user profiles, and other relevant information. The database is a NoSQL database MongoDB.

2. Email Service: Integrates with an email delivery service (e.g., SendGrid, AWS SES) to send email notifications to users, such as when a lost pet is found or when there are matching search results. (Nice to have)

3. SMS Service: If you want to provide SMS notifications, you can integrate with an SMS gateway service (e.g., Twilio, Nexmo) to send text messages to users. (Nice to have)

4. Image Storage: External cloud storage service (e.g., Amazon S3, Google Cloud Storage) to store and retrieve pet images uploaded by users.

5. External APIs: User authentication or mapping services for additional geolocation features. (Maybe)


## User Stories

## Wireframes

## Project Planning and Management


