# AirBnB Clone Project

## Project Overview

This project is a clone of the Airbnb platform, built to simulate core functionalities such as property listings, bookings, reviews, and payments. The goal is to demonstrate full-stack development skills with a strong focus on backend design, database architecture, and API security.

## Team Roles

### Backend Developer

Responsible for creating APIs, handling business logic, integrating the database, and ensuring the backend is scalable and secure.

### Database Administrator

Designs and manages the database schema, ensures data consistency, normalization, indexing, and performs regular backups.

### Frontend Developer

Implements user interfaces using frameworks like React, ensuring responsive and intuitive user experiences.

### DevOps Engineer

Handles deployment, CI/CD pipelines, and server configuration to ensure smooth delivery and scaling of the application.

### QA Engineer

Writes test cases, performs manual and automated testing to ensure code reliability and user satisfaction.

## Technology Stack

* **Django**: A high-level Python web framework for building RESTful APIs and managing server-side logic.
* **PostgreSQL**: A powerful, open-source relational database used for structured data storage.
* **GraphQL**: An API query language to fetch data efficiently and reduce the number of server requests.
* **Docker**: Used to containerize the application for consistent development, testing, and deployment.
* **GitHub Actions**: Automates testing and deployment tasks in CI/CD pipelines.

## Database Design

### Key Entities and Fields

* **Users**: `user_id`, `first_name`, `email`, `role`, `created_at`
* **Properties**: `property_id`, `host_id`, `name`, `location`, `pricepernight`
* **Bookings**: `booking_id`, `user_id`, `property_id`, `start_date`, `status`
* **Reviews**: `review_id`, `user_id`, `property_id`, `rating`, `comment`
* **Payments**: `payment_id`, `booking_id`, `amount`, `payment_date`

### Relationships

* A user can have multiple properties.
* A booking is made by a user for a specific property.
* A review is left by a user for a property they have booked.
* A payment is associated with a specific booking.

## Feature Breakdown

### User Management

Handles user registration, login, profile updates, and role-based access (guest, host, admin).

### Property Management

Allows hosts to add, update, and remove listings, including descriptions, images, and pricing.

### Booking System

Enables users to search, view availability, and book properties for specific dates.

### Reviews

Guests can leave ratings and comments after completing their stay to build trust and transparency.

### Payment Processing

Users can make payments via multiple gateways (e.g., PayPal, Stripe) for their bookings.

### Messaging

Enables communication between hosts and guests through an internal messaging system.

## API Security

### Authentication

Secure login mechanisms (e.g., JWT) ensure only authorized users access the system.

### Authorization

Role-based permissions restrict sensitive operations to the right users (e.g., only hosts can manage properties).

### Rate Limiting

Limits the number of requests to prevent abuse and protect server resources.

### Importance

* **User Data Protection**: Prevents unauthorized access to personal info.
* **Payment Security**: Ensures safe transactions.
* **System Stability**: Reduces risk from bots or malicious actors.

## CI/CD Pipeline

CI/CD (Continuous Integration/Continuous Deployment) automates the process of testing, building, and deploying applications.

### Tools

* **GitHub Actions**: Runs automated tests and deploys code on push or PR events.
* **Docker**: Ensures consistency across environments during deployment.
* **Heroku/AWS**: Hosting platform for deployment.

### Benefits

* Faster development cycles
* Fewer deployment errors
* Easier code integration and testing
