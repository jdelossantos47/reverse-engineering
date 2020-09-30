# reverse-engineering

--USER STORY-- As a user that has experienced a password security threat. This app allows users to login safely with password encryption.
 
#Technology used
#BCRYPTJS -EXPRESS -EXPRESS-SESSION -MYSQL- PASSPORT- PASSPORT-LOCAL -SEQUELIZE

#PASSWORD AUTHENTICATION-- This app allows users to login safely with password encryption.. Data is stored through the mysql database.

#Middleware:

##isAuthenticated.js  This javascript file restricts the user from using routes unless they are logged in. If the user is logged in the routes will work and process the request.
Config.json:  file that define global values and dependancies. Allows access to the database. Configuration to connect to the server 
Passport.js this contains javascript logic that tells Passport that we are trying to log in. It lets Passport know that we are using an email and password to access the page.


#Models:

##index.js this is our connection to the database using Sequelize Connects to the database and imports the users login data
user.js This requires "bcrypt" for password hashing. This makes our database secure even if it is compromised. In this file we have javascript that defines what is stored in our database.;

#Routes:

##api-routes.js This javascript file contains routes for signing in, logging out and getting users specific data to be displayed client side. 
##html-routes.js This javascript file contains routes that check whether the user is signed in. This also checks if user already has account or not, and sends them to the correct html page 
##package.json This javascript file contains all package info, version info, and node modules used
##server.js  This file requires packages, sets up PORT, creates express and middleware. This file also creates routes that syncs with database and it logs message in the terminal on successful connection to server  Creates express app and configured middleware needed for authentication
 
