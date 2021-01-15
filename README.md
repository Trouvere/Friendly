# Friendly app

## Purpose

This app allows people to stay connected within the company, find interest groups, meet new people and enjoy communication.

## Setup and run

1.  **Clone** the repository: 

2.  **server**

    2.1 Go to folder **server** and install dependency: `npm install`

    2.2 Create file named .env in `server` folder

    2.3 Put this content into the file

        SECRET =
        USER_DB =
        PASSWORD_DB =
        DB_PORT=
        DB_URL=localhost

    2.4 Start the MySQL database

    2.5 Run server: `npm run dev`

**important**: make sure you don't have server node app running before this steps, as it may lock DB and prevent DB reset

3. **client**

   3.1 Go to folder **client** and install dependency: `npm install`

   3.2 Run client: `npm run dev`

## Helpful tips

- The client will start on 3000 port (if port isn't already in use) and the server will be available on 8000 port.

## Stack:
**server**
- Node.js
- Express
- Sequelize 
- MySQL


**client**
- React
- Redux
- Formik


**tools**

- eslint
- stylelint
- prettier
- husky
- lint-staged