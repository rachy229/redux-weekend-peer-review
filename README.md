# Weekend Challenge 11 - React-Redux Feedback Form

## Instructions

Reviewing code is an important role developers play. We're going to practice reviewing code from others.

- Get the repo url from your partner
- Get your partner's project running on your computer
- Review the code from your partner and give relevant feedback
- Complete the Markdown section and submit that in the notes section on the assignment app. (Make sure you include who's code you reviewed.)

Practicing compassionate code reviews is important (you can learn more from this video on the topic: https://www.youtube.com/watch?v=Ea8EiIPZvh0 )

## Review Checklist

## Base Required Features 

- Multi-Part Form:  
  - [YES] Able to add feedback
    - [YES] Data collected on individual pages & components
    - [YES] Click on next takes you to the next page in sequence
    - [YES] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [YES] Thank you page takes you back to the first view
    - [YES] Old Data is cleared on form completion

- Client code:
  - [YES]  Individual components for each form part
  - [YES]  Redux setup complete
    - [YES] Store linked to react with `<Provider>`
    - [YES] Store setup with reducer(s) and logger middleware 
  - [YES] Reducers & Actions Working
    - [YES] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [YES] Actions have a `type` key, and `payload` if sending data
    - [YES] Reducers are returning a new state, or the old state (not mutating)
    - [N/A] Reducers are using spread correctly (to keep old data, while adding new)
  - [YES] Review Component shows at all times with current redux state
  - [YES] React-Redux Working
    - [YES] Dispatching actions onClick
    - [YES] Grabbing data from the redux store with `useSelector`
  - [YES] Axios POST request to add feedback


- Server code:   
  - [YES] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [YES] Multiple git commits showing incremental progress
  - [YES] Commits are descriptive of the changes made or feature added 
  - [YES] Has .gitignore with node_modules
  - [YSE] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [YES] Appropriate amount of code comments
  - [YES] Code is consistently formatted
- Client
  - [YES] Appropriate use of HTML tags
  - [YES] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of  _Exceeds Expectations_

- Previous Steps
  - [ ] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [ ] user can upate their score for a step
    - [ ] new score is validated to not be empty
    - [ ] redux is updated with new score
  - [ ] user can continue on to review page and submit as in Base Mode


- Admin View
  - [ ] All entries are visible with correct data from inputs
    - [ ] Most recent is at the top
  - [ ] Can Delete an entry
    - [ ] User is prompted before deleting
  - [ ] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [ ] Styling with Material UI
- [ ] Ability to flag a feedback item on `/admin` for further review
- [ ] Deployed to Heroku


## Markdown

```
Hey Tim,

General Feedback.

Looks good!

---
| Functional Requirements | Complete? |
| YES | :---: |
| Multi page form with client side routing and navigation (next button) | no |
| Data stored in Redux when navigating from page to page | no |
| User is notified when trying to leave a blank score | no |
| Review Component displays scores and comments from current redux state | no |
| Submit button sends data to the server via Axios | no |
| Confirmaion Page displays after data is POSTed to the server | no |
| Button on Confirmation Page clears Redux and starts a new survey | no |
| Views are broken down into components | no |

---
### Notes:

Notes on the above Functional Requirements.

-Could have added a min and max to the inputs, that way you don't even have the option to choose a number outside of 1-5, and only alerted for an empty value.
-Technically the comments section was listed as being "optional" so you didn't need to have the input validation there.
-README is simple and concise 
-Overall, super clean

---
| General Items | Complete? |
| YES | :---: |
| More than 15 git commits | no |
| Commits are descriptive of the changes made or feature added | no |
| Readme file updated | no |
| Appropriate amount of code comments | no |
| Code is consistently formatted | no |
| Server code organized with router & module files | no |

---
### Notes:

Notes on General Items

-very good code comments, super descriptive, makes it easy to read/understand
-could have added additional/different styling but funcionally it's all there

```
