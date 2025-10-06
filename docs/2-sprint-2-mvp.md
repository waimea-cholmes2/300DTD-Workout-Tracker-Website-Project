# Sprint 2 - A Minimum Viable Product (MVP)


## Sprint Goals

Develop a bare-bones, working web application that provides the key functionality of the system, then test and refine it so that it can serve as the basis for the final phase of development in Sprint 3.


---

## Implemented Database Schema

- Users Table Holds the info about each user, it links to the workout table to show who owns each workout, and it links to the favourites table to allow the users to favourite exercises.

- Favourites Table links to users and exercises allowing users to favourite exercises

- Workout Table holds each users workout info, links to users and exercises, to show what exercise the user did in their workout

- Exercise Table holds each exercises information, which all users can see and complete a workout with, this table links to the workout table, and the favourites table, for each user to have favourites.

![SCREENSHOT OF DB SCHEMA](screenshots/DB(1).png)


---

## Initial Implementation

The key functionality of the web app was implemented:

**PLACE SCREENSHOTS AND/OR ANIMATED GIFS OF THE SYSTEM HERE**


---

## Exercise Table

I'm getting the exercise Table to show favourites, owned and others separately, but the symbol to show the owned in the favourites I can't get to show

![Exercise not showing owned symbol](screenshots/exercise_no_own_showing.png)

### Changes / Improvements

The problem was I wasnt pulling the exercises user id to compare with the sessions user id, so i fixed that

![Exercise showing owned symbol](screenshots/exercise_own_showing.png)


---

## Favouriting and Unfavouiting exercises

I've added the favourite route and button and now i will try to favourite and unfavourite an exercise

**PLACE SCREENSHOTS AND/OR ANIMATED GIFS OF THE TESTING HERE**
![Favouriting Error](screenshots/favouriting_error.png)

### Changes / Improvements

The error was a result of me using the wrong method in my route, I was using the post method when i needed to use the GET method

**PLACE SCREENSHOTS AND/OR ANIMATED GIFS OF THE IMPROVED SYSTEM HERE**
![Favouriting Working](screenshots/favouriting.png)
![Unfavouriting Working](screenshots/unfavouriting.png)


---

## Workouts Table

I've made the workouts table to show all of the data for each workout

![Workouts Table](screenshots/workouts_table.png)

### Changes / Improvements

I showed it to my end-user to see what they thought and they reminded me I needed to add a delete button in the table, but other than that it was all good.

![Workouts Table New](screenshots/workouts_table_new.png)


---

## Deleting Workouts

I made the route for deleting workouts, and then tried to use it, the item was being delted from the table, but the return redirect waasnt working.

![Deleting Workout Fail](screenshots/delete_workouts_fail.png)

### Changes / Improvements

The problem was that i wasnt passing through the exercise id into the route, so it couldnt look for the exercise. Instead of passing it through i used request referrer to go back to the previous page

![Deleting Workout](screenshots/delete_workout.png)


---

## Testing FEATURE NAME HERE

Replace this text with notes about what you are testing, how you tested it, and the outcome of the testing

**PLACE SCREENSHOTS AND/OR ANIMATED GIFS OF THE TESTING HERE**

### Changes / Improvements

Replace this text with notes any improvements you made as a result of the testing.

**PLACE SCREENSHOTS AND/OR ANIMATED GIFS OF THE IMPROVED SYSTEM HERE**


---

## Testing FEATURE NAME HERE

Replace this text with notes about what you are testing, how you tested it, and the outcome of the testing

**PLACE SCREENSHOTS AND/OR ANIMATED GIFS OF THE TESTING HERE**

### Changes / Improvements

Replace this text with notes any improvements you made as a result of the testing.

**PLACE SCREENSHOTS AND/OR ANIMATED GIFS OF THE IMPROVED SYSTEM HERE**


---

## Testing FEATURE NAME HERE

Replace this text with notes about what you are testing, how you tested it, and the outcome of the testing

**PLACE SCREENSHOTS AND/OR ANIMATED GIFS OF THE TESTING HERE**

### Changes / Improvements

Replace this text with notes any improvements you made as a result of the testing.

**PLACE SCREENSHOTS AND/OR ANIMATED GIFS OF THE IMPROVED SYSTEM HERE**


---

## Testing FEATURE NAME HERE

Replace this text with notes about what you are testing, how you tested it, and the outcome of the testing

**PLACE SCREENSHOTS AND/OR ANIMATED GIFS OF THE TESTING HERE**

### Changes / Improvements

Replace this text with notes any improvements you made as a result of the testing.

**PLACE SCREENSHOTS AND/OR ANIMATED GIFS OF THE IMPROVED SYSTEM HERE**


---

## Sprint Review

Replace this text with a statement about how the sprint has moved the project forward - key success point, any things that didn't go so well, etc.

