Title: Copy with ssh
Date: 2022-12-10 
Category: Tips software


# ¿Qué es SSH?

SSH (o Secure SHell) es el nombre de un protocolo y del programa que lo implementa cuya función principal es el acceso remoto a un servidor por medio de un canal seguro en el que toda la información está cifrada. Además de la conexión a otros dispositivos, SSH permite copiar datos de forma segura (tanto archivos sueltos como simular sesiones FTP cifradas)

# ¿Qué es SCP?

SCP significa Copiado Seguro (Secure Copy) y es un comando que hace uso de SSH para copiar archivos de un ordenador a otro a través de una conexión encriptada.

## Ejemplos

Copiar un archivo local a un destino remoto

Fórmula:

```
scp /ruta/origen/archivo.tx usuario@ip-destino:/ruta/destino/
```

Ejemplo Práctico:

```
scp /home/user/Document/archivo.txt admin@192.168.1.1:/home/admin
```
Copiar un archivo remoto a un destino local

Fórmula:

```
scp usuario@ip-o-domninio:/ruta/origen/archivo.txt /ruta/destino/
```

Ejemplo Práctico:

```
scp root@10.0.2.12:/home/admin/user.txt /home/user/Documentos/
```

Copiar Directorios (Carpetas)

Fórmula:

```
scp -r usuario@servidor:/ruta/remoto /ruta/local
```

Ejemplo Práctico:

```
scp -r admin@192.168.1.1:/var/log/ /home/user/Documentos/
```