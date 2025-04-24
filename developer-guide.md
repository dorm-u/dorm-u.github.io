![DormU Logo](img/dormu-logo.png "DormU Logo")

* [Overview](/index)
* [User Guide](/user-guide.md)
* [Developer Guide](/developer-guide.md)
* [Development History](/dev-history.md) 
* [Contact us](/contact-us.md) <br>

# How to install and modify this project

## [Link to the Project on Github](https://github.com/dorm-u/dorm-u.github.io)

## Download Project
Open this project in Github and create a fork of the repository.

Press code button and open using Github Desktop.

*If you would like to use the raw files instead, you may download them here [not yet implemented]()*

## Setup Project
Open the project in your IDE and install dependencies using the following command in a project terminal

```
$ npm install
```

Run the system in your local environment with the following command. The website landing page should show at [localhost:3000](localhost:3000)


```
$ npm run dev
```

## Setup Postgre
The DormU application uses [PostgreSQL](https://www.postgresql.org/) to manage database and entity relationships. 

Navigate to the sample.env file and rename it to .env

Modify the .env file to point to your local postgresql server (or live server if you have one)

Run the following code to seed the database with predefined users and posts

```
$ npx prisma db seed
```

Close the running build (if it is running) using Ctrl+C on the terminal and refresh the client using 

```
$ npm run dev
```

Website should be fully functional with no errors. If something does not show then please try to retract steps. 

## Editing
Once you are complete with your modifications, run eslint to ensure that there is no typescript/javascript errors

```
$ npm run lint
```

Congratulations, you have successfully modified the DormU project code. 