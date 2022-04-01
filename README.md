# Crear Usuarios en Oracle

> This is how u can create a user in oracle

``` sql
create user myuser identify by password
default tablespace system
temporary tablespace temp
quota unlimited on system;

```
> Para que el usuario pueda iniciar sesion se le tiene que otorgar los privilegios de session.

```oracle
gran create session myuser;
```



