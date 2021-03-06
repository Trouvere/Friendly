# Friendly app

See work app: https://friendlygh.netlify.app/

See code:

**server**(https://github.com/Trouvere/FriendlyGH-server.git)

**client**(https://github.com/Trouvere/FriendlyGH-client.git)

## Purpose

This app allows people to stay connected within the company, find interest groups, meet new people and enjoy communication.

## Setup and run

1.  **Clone** the repository:

    **server**(https://github.com/Trouvere/FriendlyGH-server.git)

    **client**(https://github.com/Trouvere/FriendlyGH-client.git)
    
2.  **Run MySQL script**

    2.1 Open MySQL Command Line Client as administrator

    2.2 Enter comand:  
    
        source "directory"\"fileName".sql 

    (for exemple `source C:\Users\User\Documents\FriendlyScript.sql`)


    Or import using MySQL Workbench

3.  **server**

    3.1 Go to folder **server** and install dependency: `npm install`

    3.2 Enter password:

    3.3 At the file `\server\server.js` in the line 11 change origin

        origin: 'url client '

    (for default it will be 'http://localhost:3000')

    3.4 Put this content into the file (filling in the fields USER_DB, PASSWORD_DB, DB_PORT)

        SECRET = secret
        USER_DB =
        PASSWORD_DB =
        DB_PORT=
        DB_URL= localhost

    3.5 Start the MySQL database

    3.6 Run server: `npm run dev`

**important**: make sure you don't have server node app running before this steps, as it may lock DB and prevent DB reset

4. **client**

   4.1 Go to folder **client** and install dependency: `npm install`

   4.2 Run client: `npm run dev`

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
