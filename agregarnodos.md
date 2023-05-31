# Cómo agregar nodos a Cassandra

Para agregar nodos a Cassandra hay que cambiar algunos parámetros en el fichero de configuración **/etc/cassandra/cassandra.yaml**.

Lo primero es cambiar el nombre del clúster, que habrá que poner el mismo en cada uno de los nodos. Ese cambio se realiza con el siguiente comando dentro de Cassandra:

`UPDATE system.local SET cluster_name = 'Cluster Oscar' WHERE KEY = 'local'`

Una vez hecho eso se reinicia el servicio.

El primer parámetro que voy a mencionar el **seeds**. Este parámetro indica la lista de hosts para que puedan encontrarse entre si y aprender la topología del anillo: [Ejemplo](https://github.com/oscarmb99/Cassandra/blob/main/imagenes/seeds.PNG)

El siguiente parámetro es **listen_address**. Este parámetro se usa para indicar la dirección ip que Cassandra vincula para conectar con otros nodos. [Ejemplo](https://github.com/oscarmb99/Cassandra/blob/main/imagenes/listenaddress.PNG)

Otro parámetro a tener en cuenta es **rpc_address**. Es la dirección de escucha para los clientes. [Ejemplo](https://github.com/oscarmb99/Cassandra/blob/main/imagenes/rcpaddress.PNG)
