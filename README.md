# ![Title Header](../mafia-lite/client/src/assets/images/image132.png)

## Summer Internship 2022

### 🧑🏽‍🤝‍🧑🏼 Maintainers

- William Rodriguez
- James Fox
- Marcus Lorenzo
- Mark McConnell

## 📂 Table Of Contents

* [Description](#description)
  - [Summary](#summary)
  - [MVP](#mvp)
  - [Stretch Goals](#stretch-goals)
- [Technologies Used](#technologies-used)
- [Installation, Setup, and Running The App](#installation-setup-and-running-the-app)
  - [Installation](#installation)
  - [Required Files](#required-files)
  - [Running The App Locally](#running-the-app-locally)
- [The Nameless Terror API Reference](#the-mafia-api-reference)
- [Bugs](#bugs)
- [License](#license)

## 📝 Summary <a id="summary"></a>

_This is a full stack application that uses prisma and postgresql for the backend, node/express for the server, and react for the front-end and is written using typescript._

## ✅ Description <a id="description"></a>

_This is a web application that will allow a group of users to play a lovecraftian-styled hidden role game. It largely based off the popular games of Mafia, Werewolf and The Townspeople. The objective of the game is for the cultists to “kill” investigators until they are the majority, or for the investigators to kill off all the cultists. When one of those two things happens, the game is over and the respective faction wins!._

### 🎯 MVP <a id="mvp"></a>

- Basic game default settings
- Game logic decides roles based off of the amount of players
- A Help section and or tutorial for first time players
- A flowchart of the game and how to win(Readme)
- A user should be able to host a game
- A user should be able to join a game with an access code
- A clean & easy UI to interact with
- A manual "ready" button to move game forward
- A tooltip for roles to help remind players what their role can/can't do
- A group of user should be able to successfully start and complete a game

### ⭐ Stretch Goals <a id="stretch-goals"></a>

[] A simple tutorial toggle with persisted user preferences
[] Customizable settings
[] Mini games between rounds
[] SMS/Email invites
[] A timer
[] Custom Themes
[] In-game communication/Chat


## 🖥️ Technologies Used <a id="technologies-used"></a>

- _[React](https://reactjs.org/)_
- _[React Query](https://tanstack.com/query/v4/?from=reactQueryV3&original=https://react-query-v3.tanstack.com/)_
- _[React Router](https://reactrouter.com/)_
- _[Typescript](https://www.typescriptlang.org/)_
- _[Socket.IO](https://socket.io/)_
- _[Prisma](https://www.prisma.io/)_
- _[PostgreSQL](https://www.postgresql.org/)_
- _[ExpressJs](https://expressjs.com/)_
- _[Express-Session](https://www.npmjs.com/package/express-session/v/1.17.3)_
- _[Prisma-session-store](https://www.npmjs.com/package/@quixo3/prisma-session-store)_
- _[ViteJS](https://vitejs.dev/)_
- _[Nodemon](https://www.npmjs.com/package/nodemon)_
- _[Fly.IO](https://fly.io/)_
- _[Swagger-ui-express](https://www.npmjs.com/package/swagger-ui-express)_

## ⚙️ Installation, Setup, and Running The App <a id="installation-setup-and-running-the-app"></a>

### Setup/Installation Requirements <a id="installation"></a>

- _Please ensure you have the latest version of NodeJs and PostgreSQL_
- _Clone this repository <https://github.com/eyecuelab/mafia-lite> locally_
- _Navigate to the root folder `mafia-lite` and then `cd api` and run `npm install` and then `cd client` and run `npm install`_.
- See below for required .env files
- You will also need to have your database setup in PostgreSQL
- To ensure the prisma schema has been updated to PostgreSQL, Run a migration to create your database tables with Prisma Migrate:
    - `npx prisma migrate dev --name init`
    - `npm run seed` to seed the database with the default roles
- Also, Prisma Studio is a visual editor for the data in your database. 
  - Run `npx prisma studio` in your terminal.
### Required .env Files <a id="required-files"></a>

- In the `/api` directory, create an .env file and insert the following: `DATABASE_URL="postgresql://postgres:yourPasswordGoesHere@localhost:5432/yourDatabaseNameGoesHere?schema=yourSchemaNameGoesHere"` & `SESSION_SECRET="yourSecretGoesHere"`
- Then save
- In the `/client` directory, create an .env file (separate from the previous), and insert the following: `VITE_API_ENDPOINT=http://localhost:3000`
- Then save

### Running the App Locally <a id="running-the-app-locally"></a>

- Split your terminal into two separate consoles
- Navigate one terminal into the `/api` directory and run `npm run dev`
- Navigate the second terminal into the `/client` directory and run `npm run dev` as well. If your browser does not automatically load, type `http://localhost:5173/` manually in the browser

## The Nameless Terror API Reference <a id="the-mafia-api-reference"></a>
Everything you need to interact with our API.
### Making Requests
- In progress

- User:
  - GET `/user` retrieves all users.
  - GET `/user/:id` retrieves a single user by id.
  - POST `/user/` creates a new user.
  - PUT `/user/:id` updates a single user.
  - DELETE `user/:id` deletes a single user.

- Game:
  - GET `/game` retrieves all games.
  - GET `/game/:id` retrieves a single game.
  - POST `/game/:id` creates a new game.

- Round:
  - GET `/round/:id` retrieves specific round from game.
  - GET `/rounds/:gameID` retrieves all rounds from game.

### The Request Body
- In progress
### Models
- In progress
### [How to play](https://www.kqed.org/pop/10178/how-to-play-mafia-an-in-depth-guide-to-the-perfect-holiday-game#:~:text=Simply%20put%2C%20the%20objective%20of,happens%2C%20the%20game%20is%20over.)

## Known 🐛 Bugs <a id="bugs"></a>

* _No Known Issues_

## 🎫License <a id="license"></a>

[MIT](LICENSE) 👈

_If you run into any issues or have questions, ideas, or concerns;  please email us_

Copyright (c) 2022 - William Rodriguez - James Fox - Marcus Lorenzo - Mark McConnell
