# CPQ-Backend
* Boilerplate

### Boilerplate
1. Install __Node.js__
2. `npm init -y`
3. `git init`
4. create `.gitignore` file from Toptal Website
5. Third Party Packages
    - `npm install express` Server-side web framework
    - `npm install -D nodemon` Automatic Server Restart
    - `npm install -D dotenv` Hide sensitive information
6. create two folders :
    * __src__ : development
    * __dist__ : production
7. Setup Typescript 
    - `npm install -D typescript @types/node @types/express ts-node`
    -  `tsc --init` create __tsconfig.json__ file
    - modify __tsconfig.json__ file -> __"ourDir":"./dist"__ for tell dist folder path
    - Run the Application on watch mode -> `tsc -w`
         * It automatically generates `JS` file of `TS` in dist folder when changes in TS files.
8. Link generated `JS` file in dist folder to `nodemon ./dist/index.js`

### Start the Application
* `tsc -w`
* `npm run start:dev`


### Folder Structure
* src
   - index.js
   - app.js
   - constants.js
   * routes
      - user.route.js
   * models
      - user.model.js
   * controllers
      - user.controller.js
   * middlewares
      - user.middleware.js
   * utils
      - user.utils.js
   * db

### Explanation
- **src/**: The main directory for your source code.
  - **index.js**: The entry point of your application.
  - **app.js**: Usually where you initialize and configure your Express application.
  - **constants.js**: A place for storing constant values used across your application.
  - **routes/**: Contains all your route definitions.
  - **models/**: Contains your database models (e.g., for ORM like Sequelize or Mongoose).
  - **controllers/**: Contains the logic for handling requests and responses.
  - **middlewares/**: Contains middleware functions for Express.
  - **utils/**: Utility functions and helpers.
  - **db/**: Database-related configurations, migrations, and seeds.
