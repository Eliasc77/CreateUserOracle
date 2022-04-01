# Crear Usuarios en Oracle

> CREACION DE USUARIOS:

``` sql
create user myuser identify by password
default tablespace system
temporary tablespace temp
quota unlimited on system;
```

> PRIVILEGIOS DE USUARIO:
#### Para que el usuario pueda iniciar sesion se le tiene que otorgar los privilegios de session.
``` sql
grant create session myuser;
```

#### Privilegios para que el usuario pueda crear tablas.
``` sql
grant create table to myuser;
```

#### Privilegios para que el usuario pueda crear vistas.
``` sql
grant create view to myuser;
```

#### Privilegios para que el usuario pueda crear Procedimientos dentro de la base de datos.
``` sql
grant create procedure to myuser;
```

#### Privilegios para que el usuario pueda crear secuencias.
``` sql
grant create sequence to myuser;
```

> PRIVILEGIO PARA ADMINISTRAR TABLAS
```SQL
grant all on nombredetabla to myuser;
```

#### revocar los privilegios
```sql
revoke all on nombredetable from myuser;
```

> ELIMINAR EL USUARIO
```sql
drop user myuser cascade;
```
