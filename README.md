
> A web application built using Spring Boot to provide users with a platform to manage their favorite anime.
> The app uses the [_Jikan API_](https://docs.api.jikan.moe/) to provide up-to-date information about anime and includes features such as login/registration, anime search, top anime ratings, and more.

## Table of Contents
* [Overview](#overview)
* [Technology Stack](#technology-stack)
* [Additional Tools](#additional-tools)
* [Features](#features)
* [Local Deployment](#local-deployment)


## Overview
> Anime List is my first web development project, designed to reinforce my newly acquired knowledge after completing the cource
> This project allowed me to apply my skills and gain hands-on experience working with Java, Spring Boot, and database development.


## Technology Stack
- Java 17

- Spring Boot 2.7.7
- Spring MVC
- Spring Data JPA
- Spring Security

- Hibernate
- MySQL database
- Thymeleaf

- Javax Validation API

## Additional Tools
- **`Liquibase:`** Database migration management tool to manage changes with the database schema over time. Example: "We use Liquibase to maintain a history of our database schema changes, allowing us to easily track and apply migrations as our application evolves."
- **`Testcontainers:`** Library that simplifies integration testing by leveraging Docker containers. Example: "Testcontainers allows us to write integration tests that run in isolated Docker containers, providing a consistent and reproducible environment for testing our application's interactions with external dependencies."
- **`Hibernate Envers:`** Library for auditing and versioning of entities. Example: "Hibernate Envers helps us track changes to our entities, allowing us to audit modifications and retrieve historical snapshots of data for compliance, analysis, or debugging purposes."
- **`Spring Mail:`** An API for sending mails, from within the Spring framework. Example: "We use Spring Mail to send registration confirmation emails to users who sign up for our application, providing a seamless and automated email notification process."
- **`Lombok:`** Library used to reduce boilerplate code in Java. Used to simplify Java code by generating common boilerplate code automatically, such as getters, setters, and constructors.
- **`Swagger:`** An API documentation and testing tool. Used for documenting and testing APIs, providing a visual interface for API documentation and testing.


## Features
- Login/Registration: Users can create an account and log in, with email verification required.
- Filtered anime search: Users can search for anime by title and genres, with pagination support.
- Top anime: A list of the top-rated anime, with pagination support.
- Random anime generation: Users can generate a random anime to watch.
- Detailed anime information: Users can access information about each anime, including its trailer (if available).
- Reviews: Users can write and delete reviews about any anime, with validation for at least 5 characters.
- Anime sections: Users can add anime to sections (watching, planning, completed, on-hold, dropped) and view a list of selected anime in each section, sorted by user personal rating.
- Favourites: Users can mark anime as favourites and rate them on a scale of 1 to 10.
- Profile page: Users can upload a profile photo and view available roles.
- Admin page: A page only available to users with the admin role (currently with limited functionality).
- Encrypted passwords: User passwords are encrypted using the Bcrypt algorithm for enhanced security.


## Local Deployment
1. Clone the repository using the following command in your terminal:
2. Set up the MySQL database locally
3. Set the db properties in project's `application.properties` file:
4. Set up Gmail SMTP Server for email sender. Here's a quick tutorial on [how to do that](https://www.youtube.com/watch?v=1YXVdyVuFGA&ab_channel=Sombex).
5. Finally, insert the generated password and email username in project's `application.properties` file:
```
spring.mail.username="generated-username"
spring.mail.password="password"
```
> That's it! You should now be able to run your GitHub project locally with the correct database and email configurations.

