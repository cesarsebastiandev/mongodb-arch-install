## Instrucciones de como instalar mongodb en ArchLinux

Este es el repositorio con instrucciones del video de YouTube: [PENDIENTE](PENDIENTE) 

## Apóyanos

[Suscríbete](https://www.youtube.com/@CesarSebastianDev?sub_confirmation=1) a nuestro canal de YouTube

Donaciones por Paypal: [https://www.paypal.com/donate/?hosted_button_id=UNLT89FVZF6TE](https://www.paypal.com/donate/?hosted_button_id=UNLT89FVZF6TE)


## INICIO DE LAS INSTRUCCIONES:
---
## Actualizar el repositorio oficial de ArchLinux

```
sudo pacman -Sy
```
---

## Actualizar los paquetes ya instalados en ArchLinux

```
sudo pacman -Syu
```
---

## Clonar el repo desde AUR

```
git clone https://aur.archlinux.org/packages/mongodb-bin/
```
---

## Ubicarnos en la carpeta

```
cd mongodb-bin
```
---

## Compila e instala mongodb

```
makepkg -si
```
---


## Ver el status de mondodb
```
sudo systemctl status mongod
```
---

## Iniciar o reiniciar mongodb en este momento, solo lo arranca para esta sesion
```
sudo systemctl start mongodb
```
---
## Detener el server de mongodb
```
sudo systemctl stop mongodb
```
---

## Habilitar mongodb y que se inicie automaticamente despues de prender el ordenador
```
sudo systemctl enable mongodb
```

## Revisar version
```
mongod --version
```
## Inicias el cliente
```
mongosh
```
## Ver las bases de datos
```
show dbs
```
## Creamos una base de datos
```
use usersdb
```

## Insertamos un registro
```
db.users.insertOne({ name: "SEBASTIAN", age: 24 })
```
## Creamos una base de datos
```
db.users.find()
```

## Borramos la collection
```
db.users.drop()
```

## Muestra la collection
```
show collections
```
## Borra la base de datos
```
db.dropDatabase()
```





