## ORACLE

### Seteo de password SYSTEM para ORACLE
```
docker container exec -it oracle-local /bin/bash
./setpassword.sh contrasenia
```

### Creación de esquema BLOG para ORACLE
```
CREATE USER BLOG IDENTIFIED BY contrasenia;

GRANTALL PRIVILEGES TO BLOG;

GRANT EXECUTE ANY PROCEDURE TO BLOG;
GRANT UNLIMITED TABLESPACE TO BLOG;
```
---

## TOMCAT