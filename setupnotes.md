Greater details of this explanation:
[https://towardsdatascience.com/setting-up-postgresql-in-debian-based-linux-e4985b0b766f](Click here)



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











