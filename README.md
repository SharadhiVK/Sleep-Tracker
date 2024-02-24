# Sleep Tracker

Sleep Tracker is a mobile-friendly web application that enables you to track your sleep schedule at the push of a button (well, one tap to sleep and one to wake up). You can also see your sleep trends and "sleep debt". `yarn dev` to run the frontend and backend locally.


## Installation
Sleep Tracker will run on your browser without any installation or other work. This section is for people who want to contribute to the project.

Once you have cloned the repository, you can work on the [frontend](frontend) and [backend](backend) folders separately.

### Frontend
The frontend uses React and is hosted by [Google Firebase](https://console.firebase.google.com/u/0/). It makes calls to the backend server and also directly to the Firebase authentication portal.

In the frontend folder, run `yarn install` to install the required node modules. The frontend uses
* "react" and "react-dom" to load the website
* "axios" to make requests to the backend
* "firebase" and "react-firebaseui" to enable login
* "bootstrap", "react-bootstrap", and "reactstrap" for UI
* "moment", "react-datepicker", and "react-datetime" for the time selection widget
* "recharts" and "simple-statistics" for the graph and statistics

The files available on GitHub omit some authentication information, so you will need to replace the calls to the backend and to Firebase with dummy data.

Then run `yarn start` to run the app locally.

### Backend
The backend uses express.js and is hosted by [Heroku](https://dashboard.heroku.com/apps). It accesses the Firebase database.

In the backend folder, run `yarn install` to install the required node modules. The backend uses
* "cors" and "express" to allow the frontend to make requests
* "body-parser" to parse requests
* "firebase-admin" to access the database


Then run `yarn start` to run the backend locally.
