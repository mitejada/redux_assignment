# Streamlining our Users App

# Part 1: Refactor

Using our React full-stack Users project we created, refactor the frontend to **remove all references to state** that aren't directly connected to form inputs. Redux should be handling the entire centralized state of this application, including users, usernames, and phone numbers.

We highly recommend using almost **exactly** the architecture that we utilize in the example Posts project - the more methodical you are about recreating each detail, the easier this task will be, and a little organization and planning now will save a lot of debugging in the future.

# Part 2: Expand

Utilizing your React, Express, and Redux skills, implement the following:

- Create a `Posts` table in your database. `Posts` should be connected to `Users` via id.
- Create methods and routes in your Express app for getting, creating, and deleting Posts. You should have **at least four** methods (get all, get one, create one, delete one).
- In your React apps, create profile routes for each user based on their id (`/users/:id`).
  - Inside these routes, you should see the user's name, their phone number, and their Posts, with a form to add another.
    - Is there a method you can create in your Express apps to make it easy to get all the Posts for a single user?
  - When you add another Post, it should send that Post to the backend, adding a post connected to the User ID of the profile you're visiting.
  - After submission, posts should immediately be visible on the profile page, as well, having been added to your global Redux state.
    - This involves creating new actions, a new reducer, and new containers for this information.

# Part 3: Style

Create unique styling for your very first full-stack app. Make sure it's striking!
