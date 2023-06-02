# ¿Cómo acceder a Cassandra?

Para poder acceder a Cassandra desde el terminal se usa el comando **cqlsh**. Este comando permite acceder pero no crear elementos ni acceder con usuarios creados.

Para acceder, en el fichero de configuración hay que cambiar el parámetro **authenticator** que por defecto estará en **AllowAllAuthenticator**. Se cambia a **PasswordAuthenticator**
para acceder con usuarios creados y poder realizar acciones. Una vez cambiado este parámetro ya se puede entrar con el usuario administrador, que es cassandra.

`cqlsh 192.168.18.300 -u cassandra -p cassandra  `

[ Volver al inicio ](https://github.com/oscarmb99/Cassandra/blob/main/README.md)
