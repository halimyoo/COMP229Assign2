### COMP229-VIProgrammers-Survey-TeamProject
- - -
## DESCRIPTION 
Our project's name is VIProgrammers.
Basically, it's a customer satisfaction survey website. User can create the satisfaction survey, view them, update a survey or delete it.
- - -
## Prerequisite
Please install node_modules for running our application
- - -
## Files

* Server
  * Controllers
   * Index.js
   > Description: Functions of displaying the survey lists on home pg. Also, Login function and Display RegisterPage.


* Server
  * Config
   * App.js 
   > Description: Set up of Database, authentication, express session, view engine

* Server
  * Model
   * Survey.js 
   > Description: Create the model classes
 
 
 * Server
  * Model
   * User.js 
   > Description: require modules for the User Model         
   > Preview: 
     ```javascript
     let mongoose = require("mongoose");
     let passportLocalMongoose = require("passport-local-mongoose");

     let user = mongoose.Schema(
       {
         username: {
           type: String,
           default: "",
           trim: true,
           required: "username is required",
         },
         email: {
           type: String,
           default: "",
           trim: true,
           required: "email address is required",
         },
       },
     );
     ```
