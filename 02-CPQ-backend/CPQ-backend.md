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
