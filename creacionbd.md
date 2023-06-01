# Creación de la base de datos

Lo primero para poder empezar a trabajar con Cassandra es crear el espacio de trabajo. Para crear un keyspace se utiliza el comando:

`create keyspace if not exists "nombre  keyspace" with replication = { 'class': 'NetworkTopologyStrategy', 'replication_factor': 2};`

El parámetro **class** indica el método de replicación que se va a usar. En este caso he usado **NetworkTopologyStrategy** que indica que los elementos que se creen en este keyspace estarán replicados en cada nodo. El parámetro **replication_factor** indica que solo hay una copia de cada fila en cada nodo.

Para trabajar en el keyspace creado se usa el comando **use "nombre keyspace";** .
