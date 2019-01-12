# Express LocalLibrary Tutorial

This is practice project of [MDN Express tutorial](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs).

## Setting up MongoDB

Populate test data to MongoDB.

```bash
node populatedb.js [mongodb database url]
```

## Run app

### On local environment

Create an `.env` file and fill in the information below:

```bash
DB_HOST="mongodb database host"
DB_USER="mongodb user"
DB_PASS="mongodb password"
```

If you see the debug logs, you can add `DEBUG=express-locallibrary-tutorial:*`
line to `.env` file.

Run app on local environment.

```bash
npm run devstart
```

### On heroku

Sing in to [heroku](https://www.heroku.com/) and install the client app.
Then, run following commands in root directory of this project:

```bash
heroku login
heroku create
heroku config:set DB_HOST='mongodb database host'
heroku config:set DB_USER='mongodb user'
heroku config:set DB_PASS='mongodb password'
heroku open
```

## TODO

- [ ] Implement the `NOT IMPLEMENTED` pages.
