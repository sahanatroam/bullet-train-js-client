<img width="100%" src="https://raw.githubusercontent.com/SolidStateGroup/bullet-train-frontend/master/hero.png"/>

## Bullet Train with next.js and redux
This repository contains integration with next.js and Redux with SSR support.
Basic flow: 

- _app.js (SERVER) awaits for bulletTrain to initialise and callback with flags
- _app.js (SERVER) triggers an action with the bulletTrain state
- reducer.js (SERVER) stores the Bullet Train state in an object called config
- pages/index.js (SERVER) renders markup after Bullet Train has data for getTrait, getValue etc

- _app.js (CLIENT) initialises bulletTrain on the client with the server state setState and registers an onChange function which triggers a redux action.

## Installation 
```
npm i
```
## Running in development mode 

```
npm run dev
```

## Running in production mode 

```
npm run start
```
