# Supwarden


## Installation

Now, after installed, copy the file .env.example and rename the new one .env in root directory and in client (frontend directory)
You must update process.json variable's value in `backend directory` to match with the config in .env file

Update the variable value `JWT_SECRET`

And `IS_DOCKERIZED` to true to run with docker


## Usage

set variable's value in the recommended files

Run the following command for development 
```docker compose --env-file ./backend/.env --env-file ./frontend/.env -f docker-compose-dev.yml up --build --force-recreate```

And go in frontend directory and run 
```npm run start```



Run the following command for deployment 
```docker compose --env-file ./backend/.env --env-file ./frontend/.env up --build --force-recreate```

