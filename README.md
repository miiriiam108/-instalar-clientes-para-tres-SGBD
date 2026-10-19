# -instalar-clientes-para-tres-SGBD

## Clientes para Oracle Database (en Mint/Debian)

###  Cliente gráfico: SQL Developer

He instalado un *JDK* compatible con la versión de SQL

![Captura 1](img/Captura%20de%20pantalla%202026-10-15%20192124.png)

Comprobamos la versión 

![Captura 2](img/Captura%20de%20pantalla%202026-10-15%20192220.png)

He descargado SQL Developer para Linux

![Captura 3](img/Captura%20de%20pantalla%202026-10-16%20110543.png)

He creado un lanzador de menú para  SQL Developer 

![Captura 4](img/Captura%20de%20pantalla%202026-10-16%20115224.png)

Creación de la conexión oracle

![Captura 5](img/Captura%20de%20pantalla%202026-10-16%20115914.png)


### Cliente gráfico: VS Code y extensión SQL Developer

Descargo e instalo visual studio code
![Captura 6](img/Captura%20de%20pantalla%202026-10-19%20134455.png)

Creo las carpetas y las descomprimo

![Captura 7](img/Captura%20de%20pantalla%202026-10-19%20183840.png)

![Captura 8](img/Captura%20de%20pantalla%202026-10-19%20184026.png)


### Cliente de terminal: SQL*Plus


He descargado  Oracle Instant Client para Linux x86-64: Basic y 
SQL*Plus

![Captura 9](img/Captura%20de%20pantalla%202026-10-19%20135404.png)


Tras instalar `libaio1t64` y crear el enlace simbólico, SQL*Plus se ejecuta correctamente:

![Captura 10](img/Captura%20de%20pantalla%202026-10-19%20204107.png)


### Cliente de terminal: SQLcl




## Clientes para PostgreSQL


### Cliente de terminal: psql


###  Cliente gráfico: pgAdmin 4


## Clientes para MariaDB


###  Cliente de terminal: mariadb (o mysql)



###  Cliente web: phpMyAdmin


##  Clientes para varios SGBD


###  DBeaver Community


### Adminer


## ERRORES
- El archivo que he descargado no es .zip, es .rpm por lo que el comando

  `sudo unzip NOMBRE_DEL_ARCHIVO_SQLDEVELOPER.zip -d /opt/
/opt/sqldeveloper/sqldeveloper.sh`

no puedo ejecutarlo porque solo funciona para los.zip. Para solucionarlo he utilizado los siguientes comandos

  - `cd ~/Descargas`
  - `sudo alien -d sqldeveloper-26.2.0-186.2220.noarch.rpm`
  - `sudo dpkg -i sqldeveloper_26.2.0-186.2220_all.deb`
  - `sqldeveloper`
