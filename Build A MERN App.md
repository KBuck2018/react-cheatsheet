# Build A MERN App

### What Is A MERN App

A MERN App is a full-stack application using Mongo, Express, ReactJS, and Node. Because this is a full-stack application, you will need to incorporate two concepts, back-end deployment, and front-end deployment.

### How Do I get Started

Lets pretend you've already created a back-end application and front-end completed but aren't able to connect them. To do so is quick and easy.

##### First

We need to figure out what kind of Server Configuration we'd like to use.

* **Multi-Server** is where our front-end and back-end remain completely seperate, this allows for our backend and frontend to be worked on seperately and allowing them to not have to compete for the same resources. This will need CORS to communicate with the backend and frontend.
* **Single Server** is where everything is located in one place, which means you'll only need the one deployment and don't need to use CORS.

##### Second

Seed you data on the backend using the command

```
node db/seed.js
```

This should send all of your backend data into the database and hosts the raw data on the localHost we have set up

##### Third

We'll need to install CORS on the backend so our frontend can request the data. To do this, use

```
npm install -S CORS
```

Then on the index.js file on the backend add

```
var cors = require("cors")
```

and under

```
var app = express()
app.use(cors())
```

Your backend data should now be visible on your localhost.

### Ok so I have my backend, now what

We'll need to deploy our backend so it is always set up.

* setup Heroku using your terminal

```
Heroku create appName
```

* Configure your Heroku for a database using MLAB
* Once you've created a database in mlab use:

```
heroku config:set MLAB_URL=mongodb://<your_user_login>:<your_user_password>@ds015760.mlab.com:15760/<your_db_name>
```

* This configures the database with heroku

### Lets Get Our Front-End Built

* To get our Front-End built, run the below script in terminal

```
npm run build
```

This will minimize our front-end into something that can be deployed

### Now what

* Once we've minimized our front-end, we need to install Surge which can be done by changing out directory to build:

```
cd build
npm i -g Surge
surge
```

This will deploy your front-end to a random link it creates.

**Side Note**
As I do not plan on making a single server application I did not include the process here but if you need more info please visit the Additional Resources links below to see how.

### Additional Resources

[Building A MERN App](https://git.generalassemb.ly/ga-wdi-lessons/building-a-mern-app)
