Powerlifting App

## Vision

An app where a user can track their progress over the 3 main IPF lifts, record nutritional and exercise data that will be visible to their coach and have view their programmed exercise over the week

## User flows

### View current lifetime Personal Bests

    1. User logs in
    2. User lands on home page
    3. 3 Cards on heading that outline the users personal bests on the screen
    4. User navigates to the records page
    5. User sees personal bests table which details how heavy the personal best for each SBD and when this was achieved
    6. User sees their Max Tonnage (i.e. the combined total of all 3 lifts)

### Review current exercise in block

    1. User logs in
    2. User lands on home page
    3. User sees title of current block on page
    4. User sees current week on the page
    5. User sees next day on the block
    6. User navigates over to Training page
    7. User sees overview of this weeks training block
    8. User sees what exercises they need to on the next day of training

### Review, enter and update Nutritional data

TODO: Flesh out userflow for this

### Review, enter and update Competition data

TODO: Flesh out userflow for this

### Review, enter and update Athlete Measurement data

TODO: Flesh out userflow for this

### Record Exercise Data

TODO: Flesh out userflow for this
Rough outline

- User clicks on something like "Start Day 1."
- Gets brought to a screen that will allow a user to indicate that they've started the Day and list out all exercises that they will do that day
- User clicks on Start
- Brought on a screen that displays
  - a rest timer (with ability to +- time to the programmed time in the exercise)
  - current exercise
  - number of reps, weight and sets programmed
  - number of sets remaining
  - complete or fail set button
- when user completes or fails their set, the button is clicked and then timer will countdown from Rest Start to 0.
- Once user completes all sets programmed (number of remaining sets is 0), then the next exercise that is programmed will come on
- Once user completes all exercises, day is marked as completed
- User is prompted to add in notes for day and this is recorded alongside the day done

## Pages

Home page lists all of the users current lifetime maximum weights for their Squat, Bench Press and Deadlift in their own seperate cards.
The home page also displays d3.js graphs the weights of all the successful Squat, Bench and Deadlift lifts performed for a given block.

The weekly workout page displays the following

- The title of the current week in the weightlifting Block
- The list of programmed Days of the current weightlifting Block
  - Inside each Programmed Day there is a list of workouts
    - A workout is a exercise name, a number of sets, number of repetitions, a weight, a notes section for a user to add notes in and a completed checkbox
  - Each programmed day has a completed checkbox

The measurement page contains the following:

- the athletes current bodyweight measurement in kilograms
- a d3.js graph of the last 30 days of the athletes bodyweight.

The measurement page also contains a button to add bodyweight measurement. This brings you to a page where you fill in your bodyweight in kg and a date field that is prepopulated to todays date.

The nutrition page shows a table containing the nutritional data for the given week. The nutritional data is associated to the week of the blcok.
Each row contains the following information: Date, Calories (kCal), protein, fat, carbohydrates, fibre, water intake (L), sleep (hrs).

There is a button on the page which takes you to a new page to add a new nutritional data row. The page presents an input for each field, with the Date field pre-populated to todays date.

The competition list page contains a list of competitions that were completed and the date of when the competition was completed. Clicking into a competition shows you a page containing the following:

- a table of each attempt of the 3 major lifts
- a totals column for each type
- The date that the competition was held
- Ranking in the competition
