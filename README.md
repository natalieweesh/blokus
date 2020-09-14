# Blokus!

now you can play blokus virtually with your friends! check it out here: https://blokus.nataliewee.com/

<img src="https://media.giphy.com/media/Mam7qKLAMMrS3KEZL0/giphy.gif" alt="blokus" />

## to run the app

from the client/ folder run `npm start`

it will open in `localhost:3000`

from the server/ folder run `npm start`

the server will run on `localhost:5000`

if you want to connect the front end to the local server, make sure in Game.js you set the `ENDPOINT` variable to `localhost:5000` instead of the heroku url

## to deploy the frontend

from the client/ directory, first run `npm run build`

then make sure to copy the `_redirects` file over from client/ to client/build/

then run `netlify deploy` and when it asks which folder, enter `./build`

then run `netlify deploy --prod` and when it asks which folder, enter `./build`

## to deploy the backend

from the server/ directory commit the code and run `git push heroku master`