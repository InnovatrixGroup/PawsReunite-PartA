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

#### User Registration and Authentication

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

#### Frontend

- HTML5
- CSS with [Tailwind](https://tailwindcss.com/)
- JavaScript
- [ReactJS](https://react.dev/)

#### Backend

- [NodeJS](https://nodejs.org/en)
- [ExpressJS](https://expressjs.com/)

#### Database

- [MongoDB](https://www.mongodb.com/)
- [Mongoose](https://mongoosejs.com/docs/)

#### Deployment

- Frontend: [Netlify](https://www.netlify.com/)
- Backend: [Heroku](https://www.heroku.com/home)

#### DevOps

- [Visual Studio Code](https://code.visualstudio.com/)
- [Git](https://git-scm.com/)
- [Github](https://github.com/)
- [Notion](https://www.notion.so/product)
- [Discord](https://discord.com/)

#### Testing

- [Jest](https://jestjs.io/)
- [Supertest](https://github.com/ladjs/supertest)

#### Other tools

- [Figma](https://www.figma.com/)
- [Adobe InDesign](https://www.adobe.com/au/products/indesign.html)
- [Miro](https://miro.com/app/dashboard/)
- [Adobe PhotoShop](https://www.adobe.com/au/products/photoshop.html)

## Dataflow Diagram

### User

![Dataflow diagram - User Management](./docs/DFD-user%20management.png)

### Lost/Found Pet Posts 

![Dataflow diagram - Lost/Found Pet Post Management](./docs/DFD-pet%20post%20management.png)

### Comments

![Dataflow diagram - Comment Management](./docs/DFD-comment%20management.png)

### Notifications

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

### Personas
Three personas have been identified at the early stage of the project planning:

- A pet owner who lost their pet and needs a free and easy-to-use web application that allows them to post the lost pet's information and photos so that other users can help them find the pet.
- A person who has found a lost pet in the neighbourhood wants to post the pet's information and photos online so the owner can be reunited with their pet.
- An administrator who wants the authorisation to monitor user activities, and manage the registered users and posts.

___
### Initial User Stories

1. As a pet owner, I want to register an account, so that I can report my lost pet.
2. As a pet owner/finder, I want to report a lost/found pet by providing detailed information such as pet characteristics, last seen location, and photos, so that others can help in the search and identification process.
3. As a pet owner/finder, I want to search for lost pets based on specific characteristics such as species, breed, and colour, so that I can identify potential match with my lost/found pet.
4. As a pet owner, I want to update the status of my post regarding lost pet, so that others know that the search can be closed.
5. As a pet owner, I want to access pet care resources, so that I can educate myself and provide care for my pet.
6. As a pet owner/finder, I want to manage my user profile, so that my contact information is up to date.
7. (*Nice to have*) As a pet owner, I want to receive notifications when a potential match is found between my lost pet and a found pet, so that I can be informed about potential reunions with my pet.
8. As a pet finder, I want to leave comments on the posts, so that I can provide additional information or updates.
9. As a admin user, I want to have the ability to remove inappropriate or irrelevant posts or users from the platform, so that I can help maintain a positive and safe environment for users.

___
### Improvements

After researching the functionalities of similar products on the market, and during the development of wireframes, we found that some of the original user stories were not clearly expressed or logically sound. So some improvements have been made.

#### 1. Improved the feature for users to update the post

Before:

> As a pet owner, I want to update the status of my post regarding lost pet, so that others know that the search can be closed.

After:

> 1. As a pet owner, I want to edit my post regarding lost pet, so that I can update any missing information of my pet.
> 2. As a pet owner/finder, I want to delete my post regarding lost/found pet, so that my contact information won't be disclosed to unrelated users.

#### 2. Added clearer description of the notification type

Before:

> As a pet owner, I want to receive notifications when a potential match is found between my lost pet and a found pet, so that I can be informed about potential reunions with my pet.

After:

> As a pet owner, I want to receive ***email and in-app*** notifications when a potential match is found between my lost pet report and a found pet, so that I can be informed about potential reunions with my pet.

#### 3. Split the administrator feature into two
   
Before:

> As an admin user, I want to have the ability to remove inappropriate or irrelevant posts or users from the platform, so that I can help maintain a positive and safe environment for users.

After:

> 1. As an administrator, I want to have the authorisation to remove inappropriate or irrelevant content, such as spam or offensive posts, from the platform, so that I can help maintain a positive and safe environment for users.
> 2. As an administrator, I want to have the authorisation to remove a registered user from the database if being requested by the user, so that I can fulfill the customer's request.

#### 4. Added another user story to achieve a better customer experience.

>As a pet owner/finder, I want to be able to find the contact information of the application development team, so that I can provide suggestions about the application.

___
### User Stories After Improvements

1. As a pet owner, I want to register an account, so that I can report my lost pet.
2. As a pet owner/finder, I want to report a lost/found pet by providing detailed information such as pet characteristics, last seen location, and photos, so that others can help in the search and identification process.
3. As a pet owner/finder, I want to search for lost pets based on specific characteristics such as species, breed, and colour, so that I can identify potential match with my lost/found pet.
4. As a pet owner, I want to edit my post regarding lost pet, so that I can update any missing information of my pet.
5. As a pet owner/finder, I want to delete my post regarding lost/found pet, so that my contact information won't be disclosed to unrelated users.
6. As a pet owner, I want to access pet care resources, so that I can educate myself and provide better care for my pet.
7. As a pet owner/user, I want to manage my user profile, so that my contact information is up to date.
8. (*Nice to have*) As a pet owner, I want to receive email and in-app notifications when a potential match is found between my lost pet report and a found pet, so that I can be informed about potential reunions with my pet.
9. As a pet finder, I want to leave comments on the posts so that I can provide additional information or updates.
10. As a pet owner/finder, I want to be able to find the contact information of the application development team, so that I can provide suggestions about the application.
11. As an administrator, I want to have the authorisation to remove inappropriate or irrelevant content, such as spam or offensive posts, from the platform, so that I can help maintain a positive and safe environment for users.
12. As an administrator, I want to have the authorisation to remove a registered user from the database if being requested by the user, so that I can fulfill the customer's request.

## Wireframes

![wireframe](./docs/PawsReunite.png)
Mobile, tablet and desktop version

### Mobile Version
![mobile wireframe](./docs/PawsReunite2.png)
mobile pages and features overview

![mobile wireframe](./docs/PawsReunite3.png)
![mobile wireframe](./docs/PawsReunite4.png)
![mobile wireframe](./docs/PawsReunite5.png)
![mobile wireframe](./docs/PawsReunite6.png)
![mobile wireframe](./docs/PawsReunite7.png)
![mobile wireframe](./docs/PawsReunite8.png)
![mobile wireframe](./docs/PawsReunite9.png)

### Table Version
![Tablet wireframe](./docs/PawsReunite10.png)
tablet pages and features overview

![Tablet wireframe](./docs/PawsReunite11.png)
![Tablet wireframe](./docs/PawsReunite12.png)
![Tablet wireframe](./docs/PawsReunite13.png)
![Tablet wireframe](./docs/PawsReunite14.png)
![Tablet wireframe](./docs/PawsReunite15.png)
![Tablet wireframe](./docs/PawsReunite16.png)

### Desktop Version
![Desktop wireframe](./docs/PawsReunite17.png)
desktop pages and features overview

![Desktop wireframe](./docs/PawsReunite18.png)
![Desktop wireframe](./docs/PawsReunite19.png)
![Desktop wireframe](./docs/PawsReunite20.png)
![Desktop wireframe](./docs/PawsReunite21.png)
![Desktop wireframe](./docs/PawsReunite22.png)
![Desktop wireframe](./docs/PawsReunite23.png)

## Project Planning and Management

