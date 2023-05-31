# ¿Cómo acceder a Cassandra?

Para poder acceder a Cassandra desde el terminal se usa el comando **cqlsh**.

Para acceder por primera vez, hay que entrar con el usuario administrador por defecto y a partir de ahí empezar a crear nuestros usuarios y base de datos.

En el fichero de configuración hay que cambiar el parámetro **authenticator** que por defecto estará en **AllowAllAuthenticator**. Se cambia a **PasswordAuthenticator**
para acceder con usuarios creados y poder realizar acciones.

Una vez cambiado este parámetro ya se puede entrar con el usuario administrador, que es cassandra.

`cqlsh 192.168.18.300 -u cassandra -p cassandra  `
