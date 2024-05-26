# Repliación comandos Mongo V6
## Albert Ospina
## Hernan Hernandez

```
mongod --port 27017 --dbpath /path/to/data/db1 --replSet rs0
```
mongod: Este comando inicia una instancia de MongoDB.
- --port 27017: Especifica el puerto en el que MongoDB escuchará las conexiones. En este caso, se utiliza el puerto estándar 27017.
- --dbpath /path/to/data/db1: Especifica la ruta al directorio donde MongoDB almacenará los datos para esta instancia. Reemplaza /path/to/data/db1 con la ruta real.
- --replSet rs0: Configura esta instancia para formar parte del conjunto de réplicas llamado rs0.

  ```
mongod --port 27018 --dbpath /path/to/data/db2 --replSet rs0
  ```
Este comando es similar al anterior, pero para el nodo secundario 1. Utiliza un puerto diferente (27018) y una ruta de datos diferente (/path/to/data/db2).

```
mongo --port 27017
```
Este comando inicia el shell de MongoDB y se conecta a la instancia primaria en el puerto 27017.

```
rs.initiate()
```

```
rs.status()
```

```
rs.add("host")
```

```
rs.freeze()
```
