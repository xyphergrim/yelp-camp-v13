#RESTful Routes
name    url         verb    description
============================================================
INDEX   /dogs       GET     Display a list of all dogs
NEW     /dogs/new   GET     Displays a form to make a new dog
CREATE  /dogs       POST    Add new dog to DB
SHOW    /dogs/:id   GET     Shows info about one dog

INDEX   /campgrounds
NEW     /campgrounds/new
CREATE  /campgrounds
SHOW    /campgrounds/:id

NEW     /campgrounds/:id/comments/new   GET
CREATE  /campgrounds/:id/comments       POST

#Yelp Camp

*Add Landing Page
*Add Campgrounds Page that lists all campgrounds

#Each Campground has:
*Name
*Image

#Layout and Basic Styling
*Create our header and footer partials
*Add in Bootstrap

#Creating new campgrounds
*Setup new campground POST route
*Add in body-parser
*Setup route to show form
*Add basic unstyled form

#Style the campgrounds page
*Add a better header/title
*Make campgrounds display in a grid

#Style the Navbar and Form
*Add a navbar to all templates
*Style the new campground form

#Add Mongoose
*Install and configure mongoose
*Setup campground model
*Use campground model inside of our routes

#Show Page
*Review RESTful routes we've seen so far
*Add description to our campground model
*Show db.collection.drop()
*Add a show route/template

#Refactor Mongoose Code
*Create a models directory
*Use module.exports
*Require everything correctly

#Add Seeds File
*Add a seeds.js file
*Run the seeds file every time the server starts

#Add the Comment model
*Make our errors go away
*Display comments on campground show page

#Comment New/Create
*Discuss nested routes
*Add the comment new and create routes
*Add the new comment form

#Style Show Page
*Add sidebar to show page
*Display comments nicely

#Add User Model
*Install all packages needed for auth
    *passport
    *passport-local
    *passport-local-mongoose
    *express-session
*Define User Model

#Auth Pt. 2 - Register
*Configure Passport
*Add register routes
*Add register template

#Auth Pt. 3 - Login
*Add Login routes
*Add Login template

#Auth Pt. 4 - Logout/Navbar
*Add logout route
*Prevent user from adding a comment if not signed in
*Add links to navbar
*Show/hide auth links correctly

#Auth Pt. 5 - Show/Hide Links
*Show/Hide auth links in navbar correctly

#Refactor the routes
*Use Express router to reorganize all routes

#Users + Comments
*Associate users and comments
*Save author's name to a comment automatically

#Users + Campgrounds
*Prevent an unauthenticated user from creating a campground
*Save username + id to newly created campground

#Editing Campgrounds
*Add Method-Override
*Add Edit Route for Campgrounds
*Add Link to Edit Page
*Add Update Route
*Fix $set problem

#Deleting Campgrounds
*Add Destroy Route
*Add Delete Button

#Authorization Pt. 1: Campgrounds
*Authentication - finding out if someone is who they say they are
*Authorization - once you know who someone is you figure out what they are allowed to do (permissions)
*User can only edit his/her campgrounds
*User can only delete his/her campgrounds
*Hide/Show edit and delete buttons

#Editing Comments
*Add Edit route for comments
*Add Edit button
*Add update route

<!--/campgrounds/:id/comments/:comment_id/edit-->

#Deleting Comments
*Add Destroy route
*Add Delete button

<!--Campground Destroy Route: /campgrounds/:id-->
<!--Comment Destroy Route: /campgrounds/:id/comments/:comment_id-->

#Authorization Pt. 2: Comments
*User can only edit his/her comments
*User can only delete his/her comments
*Hide/Show edit and delete buttons
*Refactor middleware

#Adding in Flash!
*Demo working version
*Install and configure connect-flash
*Add bootstrap alerts to header

#Refactoring the Landing Page

#v13
#Dynamic Pricing Feature