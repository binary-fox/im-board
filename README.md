# I'm Board

A hybrid work/entertainment todo app. Kick it off and it will randomly give you an item from your todo list to get done,
 or an entertaining activity to do. It will then check in to see if you did your todo. If you did not it will "punish" you.

## Features

- Should have a button that provides a random task/activity at any time.
- Should allow the user to select predetermined "down" times.
- Should be able to sync with the todo-list app to get todos.
- Should be able to create fun activites
  - Should have a new user setup to ask questions to figure out what types of things user would like
    - Suggestion tool for what to add
      - "Is there a restaurant/bar you have been meaning to try out"
      - "What forms of physical activites do you prefer?"
        - "Go for a walk/bike at [ geo-locate local parks/paths ]"
        - "Do you belong to a gym/studio?"
      - "What type of diet do you have? Vegan, Veg, Keto... etc" -- finds recipeis based on that which it can suggest
  - Fun things should also be free lazy things too.
    - Should be able to sync with things like tv services to grab items from watch list
    - "text [ random person from contact-list]"
    - Try out new things
      - On predefined "down" days/times, have a chance to call a rideshare to the user's house.
        - Destination is selected from a list of businesses/locations in the user's city.
      - "try out meditation -- here is a link to a free resource"
    - "Play video game" -- from pre set list of games they have.
- Should have punishments when failing to complete activity
  - Adds money to your savings
    - Future monitization could be investment pool (like [Acorn app])
  - Donates to preselected charity of choice
  - Venmos money to friend with some message like "I'm too lazy to go out and do something today, maybe you can have fun on my behalf here is some $$"
    - Also could use this as a platform for advertising with little "via - I'm Board app (link)"
  - Could bake in monitization with 1:20 times -- or some ratio -- the money goes to app.
  - Animation like "money wheel"
  - Could scale, starting at $1, but goes up for every sequentaial fail, and resets after successful completion
- Should keep stats of completiions and failurs to complete
  - Should track addings to savings/charity
    - Should also have a little tax write-off for charity as a convenience feature

# Getting Started

First, run the development server:

```bash
yarn dev
```

# Environment Info

- Node version: 14.17.4
- Postgresql version: 12

# Installing Postgresql for Ubuntu

### Create the file repository configuration:
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'

### Import the repository signing key:
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -

### Update the package lists:
sudo apt-get update

### Install PostgreSQL-12.
sudo apt-get -y install postgresql-12

### start DB server
sudo systemctl start postgresql@12-main

Open [http://localhost:3000](http://localhost:3000)

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello).