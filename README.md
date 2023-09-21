# React + Node + MSSQL

#Getting Started with my app with NodeJS, React and MSSQL

Ensure you have docker installed. Then pull the repository and run the following command

#Do this first
Change the `CHANGEME.env` file to just `.env` and add the password of the database you want in quotes `"Example123!"`. Make sure this password meets MSSQL password requirements.
If you do not want to use the `.env` file then just change the password directly in the `yml` file. So instead of `${SA_PASSWORD}` it will be `"Example123!` if you do not want to use the `.env` file

##`docker-compose up`

This command will run the two docker files that then put React on the 3000 port and NodeJS on the 8000 port. It will also create a database on port 1433.

##`docker-compose down`

This command will remove the containers which is useful when changes are done.

To run the server ensure docker is updated with the files and in docker desktop, in images, click the run icon and type the correct port and run it. This will need to be done for both REACT front end and NodeJS backend.

#You will still need to import MSSQL into the NodeJS file to query the database in NodeJS
