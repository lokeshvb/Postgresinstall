# Postgresinstall

Download the zip file from enterprisedb.com (refer https://stackoverflow.com/questions/26441873/starting-postgresql-and-pgadmin-in-windows-without-installation)

C:\Users\blokesh\Documents\postgresql-12.0-1-windows-x64-binaries\pgsql\bin>
C:\Users\blokesh\Documents\postgresql-12.0-1-windows-x64-binaries\pgsql\bin>initdb -D c:\Users\blokesh\postgressdata -U postgres -W -E UTF8 -A scram-sha-256
The files belonging to this database system will be owned by user "blokesh".
This user must also own the server process.

The database cluster will be initialized with locale "English_United States.1252".
The default text search configuration will be set to "english".

Data page checksums are disabled.

Enter new superuser password:
Enter it again:

fixing permissions on existing directory c:/Users/blokesh/postgressdata ... ok
creating subdirectories ... ok
selecting dynamic shared memory implementation ... windows
selecting default max_connections ... 100
selecting default shared_buffers ... 128MB
selecting default time zone ... Asia/Calcutta
creating configuration files ... ok
running bootstrap script ... ok
performing post-bootstrap initialization ... ok
syncing data to disk ... ok

Success. You can now start the database server using:

    pg_ctl -D ^"c^:^\Users^\blokesh^\postgressdata^" -l logfile start


C:\Users\blokesh\Documents\postgresql-12.0-1-windows-x64-binaries\pgsql\bin>pg_ctl -D ^"c^:^\Users^\blokesh^\postgressdata^"  start
waiting for server to start....2019-10-21 15:24:21.312 IST [17092] LOG:  starting PostgreSQL 12.0, compiled by Visual C++ build 1914, 64-bit
2019-10-21 15:24:21.332 IST [17092] LOG:  listening on IPv6 address "::1", port 5432
2019-10-21 15:24:21.337 IST [17092] LOG:  listening on IPv4 address "127.0.0.1", port 5432
2019-10-21 15:24:21.500 IST [16004] LOG:  database system was shut down at 2019-10-21 15:03:29 IST
2019-10-21 15:24:22.008 IST [17092] LOG:  database system is ready to accept connections
 done
server started

C:\Users\blokesh\Documents\postgresql-12.0-1-windows-x64-binaries\pgsql\bin>