#NProject
This repository is used to sync Coalition competition


###Salam chabab,

I'd like to give some guidelines that we are going to follow from the start to the end of the project inshaalah.

First thing, we are following the pure MVC pattern, what that means?

Nothing fancy, MVC is as simple as this folder structure:
 
## Model (model):
   model homa databases li khasna nkhdmo 3lihom, had folder fih schema li we have to follow in addition l wa7ed demo folder, li we can put all the data we need on it before the data gets from the backend, the bottom line models homa databases dialna fen m storin everything about the app, to asynchronize the work between frontends and backends, the froends assume bli dik data kamla is exist fwa7ed folder named demo, every query you have to send to the database, assume like you've sent it and the data got back to you in a folder named demo, you can edit it as frontend as you wish, you can make for example a file named profile.json to store data needed and work on it until the backed api is 100% ready to use

## View (view)
 View is the frontend side, it's where all the folders and files of ReactNative will be exist, of course the npx react-native init will be run here, there will be an npm package.json in this folder to manage all the frontend components needed, to manifest all the packages a mobile app developer may need, but at a much higher level, this folder is completely isolated from the Model and Controller (api), as long as we are working with Docker there will be a docker-compose.yaml file that runs all the containers when we have to deploy it.

 Of course, this stuff is still b3iid 3lina kifach n runniw containers for each one of these services but we'll discover how on our way

## Controller (api)

Controller (api folder) basically is the work of backends, hya dik 9it3at wasl bin Model (databases) and View (frontend), it's the work of backend developers to develop a great api that nail the work and provide a documentation for front-end developers with Swagger or any api documentation tool to make the work smoother between backend and frontend


## How we are going to manage the work on Github?

Well, there will be 4 main branches

- frontend branch: all about frontend
- backend branch: cares about 2 folders (api, model)
- main branch: it should be clean until we start linking between frontend and backend
- random: random stuff, may contain assets or so about our audience, new ideas or anything

Of course no need for docker at this stage, we'll need docker and exactly our brilliant man Omar in the stage where we have to link the backend with the frontend.

Feel free a chabab to express your ideas about all of what I've said above, and also feel free to let us know if something has to be changed or there is any suggestion.

For now, let's start coding as soon as we can to finish at least the MVP the best way possible.
