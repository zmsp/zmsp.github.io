---
title:  "Postgres reset"
header:
    teaser: "images/til-page.jpg"
categories: 
  - devops
  - database
tags:
  - database
  - devops
  - software
  - postgres
---

: 
tldr: 

```
sudo su
service postgresql stop
 pg_ctl -D /var/lib/pgsql/data -l logfile start
```

## To verify that the database is running 

```
database-# ps aux | grep post

## Reset process


Warning: This process supposed to delete all postgres data and configuration  

#### Run The following: 

Note: replace X.x with version number

```
sudo su
service postgres-X.x stop # stops postgres services  
rm –rf /var/lib/pgsql/X.x/data/*
sudo service postgresql-X.x initdb
service postgres-X.x start
```

## Additional info
The database connection will be lost until `data/pg_hba.conf` is configured. To allow all connection we add `host all all 192.168.0.0/24 trust` on `/var/lib/pgsql/X.x/data/pg_hba.conf`. This translates to allow type host to allow connection to all database, using any user, from ip range of 192.168.0.0 – 192.168.255.255, without any credentials.

## To only reset system password
To just reset the password instead of deleting all the configuration & data-


#### Run The following: 

```
sudo -u postgres psql
\password
Enter new password twice 
\q
```
