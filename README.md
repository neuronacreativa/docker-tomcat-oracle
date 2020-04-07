# Docker-tomcat-oracle
Docker compose for Tomcat 8.5 + Oracle 11g environment

## ORACLE

### Setting password for SYSTEM user
```
docker container exec -it oracle-local /bin/bash
./setpassword.sh password
```

### Schema creation
```
CREATE USER BLOG IDENTIFIED BY password;

GRANTALL PRIVILEGES TO NEW_SCHEMA;

GRANT EXECUTE ANY PROCEDURE TO NEW_SCHEMA;
GRANT UNLIMITED TABLESPACE TO NEW_SCHEMA;
```
---
