
### Installation (Debian)


Installs PostgreSQL and PostgreSQL client
```
apt-get install postgresql postgresql-client
```

Installs PostgreSQL documentation
```
apt-get install postgresql-doc
```

Installs PostgreSQL administration GUI
```
apt-get install pgadmin3
```

Installs PostgreSQL web-based administration tool
```
apt-get install phppgadmin
```

---

### Creating/altering/deleting roles

create role
```
CREATE ROLE examplerole WITH LOGIN PASSWORD 'password0' CREATEDB
```

drop role
```
DROP ROLE exampletole
```

---

### User access

Connect to the database
```
psql
```
Connect to localhost as mypostgresuser
```
psql -d mypostgressdatabase -U mypostgresuser
```

---


### PostgreSQL basic prompt commands

List roles
```
\du
```
List all databases
```
\l
```
List tables in connected database
```
\dt
```
List schemas
```
\dn
```
List columns on table
```
\d table_name
```
List functions
```
\df
```
List views
```
\dv
```
Pretty-format query results
```
\x
```






