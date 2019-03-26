---
layout: post
title:  "Creación de una app con express-generator"
date:   2019-03-21 16:52:26 +0100
categories: Node express
---
En esta entrada voy a explicar como generar de la manera mas rápida y simple la estructura de una aplicación del popular framework  de Node, **Express.js**.

Lo primero que necesitamos es tener instalado Node en nuestra máquina. Podemos descargar gratuitamente
la última versión desde su  [página oficial](https://nodejs.org/es/). Una vez instalado debemos abrir una terminal de comandos en nuestro sistema e instalar de manera global **express-generator** , escribiendo lo siguiente:
```
 npm install express-generator -g 
```
Ahora generamos la estructura del proyecto mediante el siguiente comando:

    express nombredemiapp

Podemos utilizar el modificador *--view* si queremos cambiar el motor de vistas por defecto que ofrece express, normalmente suele ser *jade*. 

 Si por ejemplo qusieramos cambiar el motror a pug tendriamos que escribir lo siguiente:

    express --view=pug nombredemiapp
    
Dentro de nuestra carpeta del proyecto ahora tenemos que instalar las dependencias indicadas en el *package.json*  con el siguiente comando:

    npm install

  Finalmente para arrancar la aplicación en modo debug en windows  escribimos lo siguiente:
  

    set DEBUG=myApp:* & npm start

Por defecto la aplicación se levanta en el puerto 3000 de nuestra máquina, esto podemos cambiarlo en el fichero bin/www.
