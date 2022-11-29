## Persistence and Analytics Fundamentals - Workshop Day 2
### A simple CRUD application

### Commands for mySQL
1. cd into sql folder
2. use rsvpdb
3. commit;

### Steps on mySQL Workbench to note

drop database if exists rsvpdb;

create database rsvpdb;

use rsvpdb;
CREATE USER 'rsvp'@'localhost' IDENTIFIED BY 'Password@123456';

GRANT ALL PRIVILEGES ON *.* TO 'rsvp'@'localhost' WITH GRANT OPTION;

FLUSH PRIVILEGES;

### Functions of the application
1. list all records using getAllCustomer through /api/rsvp
2. get total count through /api/rsvp/count
3. insert a new entry using insertRSVP with a POST request.
4. edit and update an entry using updateRSVP with a PUT request.