# Sharing Bill Application

Sharing Bill Application is a finance management tool designed to simplify adding bills and splitting expenses among group members. It offers features for adding, updating, deleting expenses, and settling balances. With advanced functionalities for splitting equally, unequally, by shares, and by percentages, Sharing Bill Application is the ideal tool for managing shared finances efficiently within a group.

## Overview

In this update, Sharing Bill Application introduces a new feature for sending invitations to existing users, allowing them to accept or decline the invitation.

## How it Works

- **Invitation System**: Users can send invitations to existing users to join their group.
- **Accept or Decline Invitations**: Receiving users have the option to accept or decline the invitation.

## Features

- **User Authentication**: Secure user registration and login functionalities.
- **Bill Management**: Easily add, edit, and delete bills with descriptions, amounts, and involved members.
- **Expense Splitting**:
  - **Equally**: Split expenses evenly among participants.
  - **Unequally**: Customize each participant's contribution.
  - **Shares Split**: Determine contribution shares.
  - **Percentage Split**: Specify contribution percentages.
- **Balance Settlement**: Track who owes money and who is owed.
- **Validation**: Ensure bills and expenses are correctly input and calculations are accurate.
- **Expense Filter**: Search and filter expenses with a date range.
- **Expense Pagination**: Manage and view expenses at your own pace.

## Technologies Used

- **Frontend**: Angular for building dynamic and responsive user interfaces.
- **Backend**: Node.js with Express for server-side logic and API endpoints.
- **Database**: MongoDB for flexible and scalable data management.
- **Authentication**: JWT for secure and efficient user authentication and authorization.

## Setup Instructions

### Frontend (Angular)

1. Navigate to the frontend directory:
    ```bash
    cd splitIt-app
    ```
2. Install dependencies:
    ```bash
    npm install
    ```
3. Start the Angular development server:
    ```bash
    ng serve
    ```
4. Open your browser and go to `http://localhost:4200` to access the Sharing Bill Application frontend.

### Backend (Node.js with Express)

1. Navigate to the backend directory:
    ```bash
    cd server
    ```
2. Install dependencies:
    ```bash
    npm install
    ```
3. Add a `.env` file with the following content:
    ```
    ACCESS_TOKEN_SECRET='123'
    REFRESH_TOKEN_SECRET='123'
    ```
4. Configure the MongoDB connection in `server.js`:
    ```javascript
    mongoose.connect('mongodb://127.0.0.1:27017/SplitIt', {
      useNewUrlParser: true,
      useUnifiedTopology: true,
    });
    ```
5. Start the server:
    ```bash
    node server.js
    ```
6. Test the server's API by making requests to `http://localhost:4200` using Postman or any other endpoint testing platform.

