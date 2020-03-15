---
layout: post
title:      "My Sinatra Project Journey"
date:       2020-03-15 22:23:47 +0000
permalink:  my_sinatra_project_journey
---



The name of my Sinatra app is **PillPoP**. I know it sounds really strange but indulge me for a moment if you will.  The app is designed to help people keep track of their prescription medications. The inspiration for this idea came from the fact that I am a primary caregiver to my eighty-two year old father; hence the pop in pillpop, and I help keep track of his daily medications.  The project requires a has many and a belongs to relationship with the data base. Therefore, in this case each patient has many medications and a medication belongs to a patient. Also, this app is to have CRUD features; create, read, update and delete. 

To start off, I used the Corneal Gem to setup the file system convention normally associated with Sinatra apps. This really cuts corners, because it comes packaged with all the gems required to fully implement the app. So right out of the box, we have our Model, Views and Controller files. We also have the public folder for storing images, javascript and stylesheets, as well as the config folder that stores the environment.rb file. The gem file as mentioned not only includes the Sinatra gem, but also active record, sqlite and rake, which are instrumental in managing the database. 

I created a database with users table and a medications table. The users table had rows for username, email and password_digest. One might wonder why the password_digest was used instead of just plain ole password. The reason for this is the bcrypt gem which does some really great password encryption prior to storing the password in the database. This provides a huge layer of security for the user creating the account. The medications table has a row for the medications entered by the user, and  it has a user_id row, which identifies a user to the specific medication; hence that belongs to relationship.

If this app was a car then the config.ru would be the ignition switch that starts the motor. Within the config.ru the run ApplicationController starts the motor running and instructs the program to use the MedicationsController and the UsersController. Inside the ApplicationsController are initial configuration instructions to set the use for the Public folder, to set the views folder and to enable and set sessions. The sessions are what initializes a cookie each time a user logs in, which not only provides a high level of security, but also prevents the user from having to login into every single page associated with his or her user account.

As the name suggests, the users controller, functions as the interface to login, or signup for a new account. There are error handlers built in, that prevent someone from logging in with unverified username and passwords. Also, I included code that allows a user to log out. When this happens, the session information is cleared out, which requires the user to re-log in if they want to go back to their account. Once logged in, the user controller sends a page to the user that lists all the medications they have added or a link is provided to add new medications, which takes us to the medications controller.
![](http://)
The medications controller as you may have guessed posts the medications that a user has added to his account, but only if the user has added medications. If the user has not added any medications, the user is given the option to add a new medication. Finally, I wanted the user to be able to not only add new medications, but also to be able to edit and delete a medication. These two processes are handled by the delete and patch commands. Once a delete or an edit takes place, the user is again redirected to an updated list of his or her medications.  In a nutshell the user and medications controllers, handle the create, read, update and delete functions specified in a CRUD app.

As the name implies, the views folder handles all the web page code that the users will be looking at and interacting with. I used a layout sheet as template for all the pages that user might visit. I actually created the html in Dreamweaver software because I really like the live view feature. I also created the stylesheet with Dreamweaver software as well. 

In the public folder, I have stored my images, stylesheet and favicon. I created a logo and favicon using Adobe Fireworks software. The logo and favicon were added to the layout sheet so that all the pages being visited would have a similar look. 

The app is a very simple crud app, that incorporates some useful elements. However, If I had more time, I would like to extend it even further. First, I would have a timer for medications that are taken at a specific time of day. The timer could set off an alarm, or send a text message to let the user know it is time to take their prescription. Also, I would like the medications list, to only reflect the medications that the user hasn’t taken yet on a given day.  So each time a user takes a particular medication, they can check it off and it no longer appears in the list for the rest of that period.

Finally, I am including the github repository: https://github.com/syntax4code/pillpop.git, and invite all code warriors to clone and play around with it. Have fun and thank you for reading my blog!

