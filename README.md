<!-- readme adapted/inspired from @SamuelDAlencar -->
# Ebyrt Task Manager

Task manager allows users to view all tasks in the database, update the current state between 'done, pending or ongoing', add a new one, or delete an existing one.
(option to edit/remove tasks to be implemented).

# Stacks used

- React
- ContexAPI
- Docker
- Express.js
- Typescript
- Node.js
- MySQL
- Joi
- EsLint

# How to run the application:

* Clone this repository: `git clone git@github.com:lkotlarenko/Task-Manager-App.git` (SSH)
* Enter the app folder (Task-Manager-App)
 > You can run the application on dockers containers
 > _To do this you will need docker & docker-compose_
* Run these steps in order:
1. Rename '.env.example' to '.env' and change the environment variable for DB password
2. Run 'docker-compose up -d' in the terminal
3. With the containers running healthy, attach to the backend one with `docker container exec -it app_backend sh` and run `npm run db:restore` to generate default DB
4. _if node_modules from frontend/backend wasn't created with docker-compose you can attach to the containers (see commands below) and execute `npm i`

# Useful commands

 - `docker container exec -it app_backend sh` | attach shell to backend container
 - `docker container exec -it app_frontend sh` | attach shell to frontend container

# WIP

- App test coverage on backend & frontend
- Frontend CSS using tailwind
- Public Deploy
