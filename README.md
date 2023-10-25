# e-commerce-db
This db utilizes express and sequelize using PUT, POST, and DELETE functions to manage a business stock, and  prices.

# installing

First clone the git repo off the following link:

https://github.com/julianlosak/e-commerce-db

open VS code and clone the repo.

cd into the main directory

run the following commands in the terminal:

npm init-y
npm install

Then cerate you .env file and input your MySQL password and "root" for the user section

DB_NAME='ecommerce_db'
DB_USER=''
DB_PW=''

input the follwoing command and fill out your password when prompted:

mysql -u root -p


After that is complete we have to source the schema run the following in the MYsql terminal:

source db/schemal.sql;
quit;

now we must seed the data run

npm run seed

once succesfully seeded run 

npm start

# Usage

open insomnia to acces the database

Use the following: localhost:3001/api/products, localhost:3001/api/tags, or localhost:3001/api/categories in the URL.