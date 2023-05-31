# Instalación de Cassandra

Para instalar Cassandra hay que seguir los siguientes pasos:

- Instalar las dependencias de java.

`apt install openjdk-11-jre `

- Descargarse la clave pública y agregar los repositorios.

`curl https://downloads.apache.org/cassandra/KEYS | apt-key add - `

`echo "deb https://downloads.apache.org/cassandra/debian 40x main" | tee -a /etc/apt/sources.list.d/cassandra.list  `

- Actualizar los paquetes.

`apt update  `

- Instalar Cassandra.

`apt install cassandra  `
