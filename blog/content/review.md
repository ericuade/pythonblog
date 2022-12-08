Title: Install HTOP
Date: 2022-12-03 10:20
Category: Installation software

# Como instalar HTOP en centos 7

Si queremos instalar htop para poder monitorizar que esta pasando en nuestro linux centos tenemos que realizar unas cosas previas.

Abre una terminal y usa un usuario con permisos de **root**

Instala el epel repository usando esta instruccion:
```
yum -y install epel-release
```
Refresca el epel repo con esta instruccion: 
```
yum repolist
```
Instala packages from epel repo: 
```
yum install pkg1
```
Por ultimo
```
yum install epel-release
```
Instalar HTOP
```
yum install htop
```
Ejecutar
```
htop
```
