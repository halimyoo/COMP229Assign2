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
     ```js
     const { ObjectId } = require('mongoose');
let mongoose = require('mongoose');

// create a model class
let surveyModel = mongoose.Schema({
    name: String,
    owner: String,
    user: {
        type: mongoose.Schema.Types.ObjectId,
        ref: "User"

    },
    startDate: Date,
    endDate: Date,
    q1: String,
    q1ans1: String,
    q1ans2: String, 
     ```
