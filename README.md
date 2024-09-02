# Supwarden


## On develop

Run the following command, open two command line terminal

On the first terminal, run:

- ```cd back```
- ```npm install```

Now, after installed, copy the file .env.example and rename the new one .env in root directory and in client (front directory)
You must update process.json variable's value in `back directory` to match with the config in .env file

Update the variable value `JWT_SECRET`

Do the following command to run

- ```npm run start```

On the second one, run:

- ```cd front```
- ```npm install```
- ```npm run start```


## Usage

set variable's value in the recommended files

Run the following command for development 
```docker compose --env-file ./backend/.env -f docker-compose-dev.yml up --build --force-recreate```

And go in frontend directory and run 
```npm run start```



Run the following command for deployment 
```docker compose --env-file ./backend/.env --env-file ./frontend/.env  up --build --force-recreate```

