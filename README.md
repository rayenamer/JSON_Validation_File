# SocialMedia App (DatingApp) API Collection

This README provides an overview of the **SocialMedia App (DatingApp)** API collection, designed for testing and interacting with the backend services. The collection facilitates various operations such as user registration, login, fetching user data, and managing user photos.

## Table of Contents

- [Overview](#overview)
- [Collection Details](#collection-details)
- [Environment Variables](#environment-variables)
- [API Endpoints](#api-endpoints)
- [Testing](#testing)
- [Personalization](#personalization)
- [License](#license)

## Overview

The **SocialMedia App (DatingApp)** API collection is built using Postman and contains a series of requests that allow developers to interact with the backend. The collection includes endpoints for user management, authentication, and error handling.

## Environment Variables

The collection uses the following environment variable:

- **`url`**: The base URL for the API. Default value is `https://localhost:5001`.

## API Endpoints

The collection includes the following parts and endpoints:

### Part 2: User Data Retrieval
- **Get Weather Forecast**: `GET /weatherforecast`
- **Get Users**: `GET /api/users`
- **Get User**: `GET /api/users/{id}`

### Part 4: User Registration and Login
- **Register User**: `POST /api/account/register`
- **Login User**: `POST /api/account/login`
- **Get Users**: `GET /api/users`
- **Get User**: `GET /api/users/{id}`

### Part 7: Error Handling
- **Get Null Reference Error**: `GET /api/buggy/server-error`
- **Get Auth Error**: `GET /api/buggy/auth`
- **Get Not Found Error**: `GET /api/buggy/not-found`
- **Get Bad Request**: `GET /api/buggy/bad-request`
- **Get Validation Error**: `POST /api/account/register`

### Part 8: User Management
- **Get User With Bearer Token**: `GET /api/users/{id}`

### Part 10: User Profile Updates
- **Update User**: `PUT /api/users`

### Part 11: Photo Management
- **Add Photo for User**: `POST /api/users/add-photo`
- **Set Main Photo**: `PUT /api/users/set-main-photo/{id}`
- **Delete Photo**: `DELETE /api/users/delete-photo/{id}`

### Part 12: User Registration with Additional Fields
- **Register User**: `POST /api/account/register`

### Part 13: User Likes
- **Add Like**: `POST /api/likes/{id}`
- **Get Liked Users**: `GET /api/likes?predicate=liked`
- **Get Liked Users Liked By**: `GET /api/likes?predicate=likedBy`
- **Get Liked Users Mutual**: `GET /api/likes?predicate=mutual`

### Part 15: Messaging
- **Create Message**: `POST /api/messages`
- **Get Messages**: `GET /api/messages`
- **Get Message Thread**: `GET /api/messages/thread/{username}`

### Part 18: Admin Functions
- **Get Users with Roles**: `GET /api/admin/users-with-roles`
- **Edit Roles for User**: `POST /api/admin/edit-roles/{username}`

## Testing

The collection includes tests for various endpoints to ensure they return the expected results. You can run the collection in Postman to execute the tests and view the results.

## Personalization

To use this collection effectively, you need to personalize it for your own use case. You can also utilize the project available in my repository, **SocialMediaProjectApi**, which contains the necessary backend setup and additional resources to help you get started.

## License
Feel free to use this collection as you wish!
