## Problem - Backup
In this scenario, you are requested to access the file directory specified on the machines allocated to you and prepare a scenario in which you perform backup operations in accordance with the instructions below.
### Information
Backup means backing up a database or data. A backup is an important step in protecting your data and restoring it in case of possible data loss.
The backup operation in PostgreSQL involves creating a backup file by copying the current state of the database. This backup file contains the database's data, tables, indexes and other components. The backup file can be used in situations such as moving a database to another server, recovering data or restoring it in case of data loss.

In this scenario, we will create a PostgreSQL database running in the Alpine image and then create a table and take a backup via terminal.

### Instructions
1. Go to a directory `/home` in the home directory.
2. Let's run the `docker run --name mypostgresdb -e POSTGRES_PASSWORD=mysecretpassword -p 5432:5432 -d postgres` command to boot the Postgresql database with the docker image.
3. After making sure that the Docker image is running, let's run the `docker exec -it mypostgresdb bash` command to access the postgresql database.
4. By running the command `psql -U postgres` the connection is made and you can run psql commands there.
5. After connecting to the Postgresql database, we will run the commands below to create a table and take a backup via terminal.
6. Create a new database named `mydatabase` then connect to your database by saying `\c mydatabase`.
7. After the connection is made, create a new table and run the `psql -U postgres -f create_table.sql` command to create the table using the created SQL file and exit psql with the `\q` command.
8. After the table is successfully created, you can also perform a backup using the `pg_dump` command.
9. After completing the procedures, press the "Check" button and complete the scenario.

### Successful Output
  Condition:
`` echo
[root@node1 ~]$ cat backup.sql
```