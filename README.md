# Postgres setup notes for linux/unix systems

Greater details of this explanation can be found here:
[link to detailed linux postgres setup](https://towardsdatascience.com/setting-up-postgresql-in-debian-based-linux-e4985b0b766f)



## setting up postgress server on linux or unix system


#### Add necessary software - should be available in native repositories
```
sudo apt update

sudo apt install postgresql postgresql-contrib

```

installation of postgres automatically creates a postgres user with access to a default postgress database

#### Switch to user: 'postgres'
```
$ sudo -i -u postgres

postgres@server:~$ psql

```

#### Now it's time to set up a user account

```
postgres@server:~$ createuser --interactive
```
Note: It might be a good idea to create a username with the name as the username of system you're on.

#### Accessing a database

```
$ psql {database_name}
```
Your username must first have been granted access to the database in question

You can also specify which role you want to access a database as:
```
$ psql -U {role/username} {database_name}
```

#### Creating a new database

As the postgres user, execute the following command replacing {dbname} with the desired name of your database.
```
postgres@server:~$ createdb {dbname}
```

#### Loading a database with a .sql file



```
$ createdb -U {username} {dbname}

$ psql {dbname} < {filename}.sql
```


Final note: once at a promp use '\h' to request help information






