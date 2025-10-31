# Sprint 1 - A Working UI Prototype


## Sprint Goals

Develop a prototype that simulates the key functionality of the system, then test and refine it so that it can serve as the model for the next phase of development in Sprint 2.

[Figma](https://www.figma.com/) is used to develop the prototype.


---

## Initial Database Design

- Users Table Holds the info about each user, it links to the workout table to show who owns each workout, and it links to the favourites table to allow the users to favourite exercises.

- Favourites Table links to users and exercises allowing users to favourite exercises

- Workout Table holds each users workout info, links to users and exercises, to show what exercise the user did in their workout

- Exercise Table holds each exercises information, which all users can see and complete a workout with, this table links to the workout table, and the favourites table, for each user to have favourites.


![SCREENSHOT OF DB DESIGN](screenshots/DB(1).png)


### Required Data Input

- The First data that will be input by the user will be them signing in or registering through the sign in and register form page

- The user can input a workout of an exercise of their choice, they will input the reps, sets an weight they did for the workout in the add progress form, they can also delete any progress they want in the exercises page

- The user will be able to add and delete exercise, using a the exercise adding form, and a button found on the exercises page for deleting, but only owned exercises can be deleted.

- The user will be able to favourite exercises, by clicking a button inside the exercises page

### Required Data Output

- When the user signs in a small piece of text will be displayed on the home screen, welcoming the user using their name

- When a user adds their progress to an exercise a small piece of text on the screen will displaying saying their progress has been added,  this will also update the table or graph showing the users progress, when deleting progress the user will be asked if they are sure when they press the button, then if they press ok a small piece of text will showup saying the delete was successful and the progress will be gone.

- When the user adds an exercise a small piece of text will show up saying it was successful, when deleting an exercise the user will be asked if they are sure when they press the button, then if they press ok a small piece of text will showup saying the delete was successful and the exercise will be gone

- When an exercise os favourited, the exercise will be moved up wit the other favouited exercises on the home page, and inside the exercises page their will be some symbol/button to show that it is favourited.





### Required Data Processing

Replace this text with a description of how the data will be processed to achieve the desired output(s) - any processes / formulae?
- When a user registers an account in the system, their name, username and password are sent to the server where the password is hashed and stored to protect user privacy

- When logging in the system checks the input username and password with the ones in the database, if it matches with a registered user it creates a session for the user, allowing personalised data to load

- When a user adds a workout the system links their user id and the exercise's id to the workouts table and ensures all of the correct data will be input

- When deleting a workout the system will compare the users id to the user id of the workout being deleted, to ensure that it is being deleted by the owner

- When a user adds a new exercise the system will store all of the info of the exercise like name and description, while linking the users id to the table.

- The exercises will be sorted into 3 categories favourites, owned and others, depending on their state

- When a user clicks the favourite button the system will check if the exercise is already favouited then will either favourite or unfavourite depending if it is or isnt favourited


---

## UI 'Flow'

The first stage of prototyping was to explore how the UI might 'flow' between states, based on the required functionality.

This Figma demo shows the initial design for the UI 'flow':

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://embed.figma.com/proto/wWu3U0kbDr9z01quCmicou/Workout-Tracker-App?node-id=2-37&p=f&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=1%3A2&embed-host=share" allowfullscreen></iframe>

### Testing

I took my user through the UI and explained how it will work and where everything will be
They said "Yeah thats perfect, just add like a login and register page as well"

### Changes / Improvements

- Added Login Page

- Added Register Page

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://embed.figma.com/proto/TlIZvG8s3XhFWL2VT6ufYy/Workout-Tracker-App-2-?node-id=2-22&p=f&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=1%3A2&embed-host=share" allowfullscreen></iframe>


---

## Initial UI Prototype

The next stage of prototyping was to develop the layout for each screen of the UI.

This Figma demo shows the initial layout design for the UI:


<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://embed.figma.com/proto/5ahZ8lLNkOJlpjBCUqFbMm/Workout-Tracker-High-Quality?node-id=9-141&p=f&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=2%3A2&show-proto-sidebar=1&embed-host=share" allowfullscreen></iframe>

### Testing

I moved through the design with my end user seeing if it all flowed well

My end user said " yeah it looks fine but i reckon you need a way to tell which is a favourite instead of ot being on top, like put a header or something, and also I'd need a way to see which exercises are mine, also would definitelyt need a logout button, and a way to delete the exercises I own. Also change the back button to like a home symbol in the top or something. And also maybe centre the Name in the header"

### Changes / Improvements



- List of Favourites, Owned and Other exercises, with a small symbol and key showiing which favourites are owned
- Added delete button for exercises which are owned by the user.
- A new home symbol in the top replaces the back button in certain pages, also include the home button in the forms 
- Centred the text in the header and added a logout button, as well as a login button in the header on the landing page.

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://embed.figma.com/proto/qfNz3wUZ3utSq7v1vSiOK5/Workout-Tracker-High-Quality--3-?node-id=2-2&p=f&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=2%3A2&show-proto-sidebar=1&embed-host=share" allowfullscreen></iframe>


---

## Refined UI Prototype

Having established the layout of the UI screens, the prototype was refined visually, in terms of colour, fonts, etc.

This Figma demo shows the UI with refinements applied:

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://embed.figma.com/proto/LqL4PXdQsnHulH70Sk5G3n/Workout-Tracker-Refined?node-id=2-2&p=f&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=2%3A2&show-proto-sidebar=1&embed-host=share" allowfullscreen></iframe>

### Testing

I took my end user through the UI, using all of the features so they could have an understanding of it and see if it flows well.
My end user said "Yeah it looks pretty good and flows well, but the colour is not very good, I feel like it should have darker and more aggressive colours, like black and red, you also need to add a way to favourite it in the page"

### Changes / Improvements

- Changed to more aggressive colours, using a general base of black and red, with buttons being orange

- Added a star symbol in the exercises page, where it can be clicked to favourite the exercise, filling in the star



<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://embed.figma.com/proto/dDIBsYsHW19oKQQkdwt5LJ/Workout-Tracker-Refined--2-?node-id=5-95&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=2%3A2&show-proto-sidebar=1&embed-host=share" allowfullscreen></iframe>


---

## Sprint Review

This Sprint has helped heavily to move the project forward, as it has lead me to the final design of the website, after getting feedback from my End-User.

Key success points:
- A final prototype has been made with a full UI and Flow, it runs exactly hoe the website is intended to.
- The final prototype incorporates lots of feedback from the End-User, with many improvements being made from their requests.

Challenges:
- I struggled with coming up for a general colour scheme for the website, until the End-User helped

Overall sprint1 has helped create a strong prototype to take into sprint 2, with valuable User feedback and testing.

