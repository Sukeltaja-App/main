# Info for future developers

Here is a brief guide for the next developers.
The project consists of three diffrent repositories [Backend](https://github.com/Sukeltaja-App/sukeltaja-backend),
[Frontend](https://github.com/Sukeltaja-App/sukeltaja-frontend)(Mobile-frontend) and
[Back office](https://github.com/Sukeltaja-App/sukeltaja-bo)(browser-frontend).


Main language: **Javascript**

Tools and frameworks used:
* [React Native](https://facebook.github.io/react-native/)
* [React](https://reactjs.org/)
* [Expo client](https://expo.io/)
* [Node.js](https://nodejs.org/)

---
* [Mongoose js](https://mongoosejs.com/)
* [Express js](https://expressjs.com/)

## Where to start

After fetching the repositories you need to install all the required tools.
This can be done on by typing ```npm install``` on the root folder (Node needs to be installed before).

Backend can be started with ```npm run watch``` to run in development mode.    
Frontend can be started with ```npm start```

### Backend

* Backend runs currently on [Heroku](https://www.heroku.com/) and data is stored in MongoDB @ [Mlab](https://mlab.com/).
* Back Office build runs at Backend root.
* Enviroment variables are load with [Dotenv](https://www.npmjs.com/package/dotenv) from .env file. These values are used and set at config.js file for backend.
* Testing backend is done with [Supertest](https://www.npmjs.com/package/supertest).
  - Testing uses currently real database @ [Mlab](https://mlab.com/), and sometimes fails when two sets of same tests run simultaneously. (Eg. pullrequests testing current branch + merge branch)
  - Tests create and store mock data to database before and during the tests.
* Tokens are created with [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken).