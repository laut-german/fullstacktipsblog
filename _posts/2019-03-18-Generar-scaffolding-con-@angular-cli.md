---
layout: post
title:  "Creación de una app con CLI de Angular"
date:   2019-03-26 11:49:26 +0100
categories: Angular 7
---

En el momento de escribir estas lineas la versión de Angular y @angular-cli que estoy utilizando son la **7.2.11** y **7.3.6** respectivamente. Para instalar el *command line interface* de Angular podéis hacerlo mediante npm:

    C:\> npm install -g @angular/cli

Para verificar que se ha instalado correctamente, abrimos otro terminal y escribimos el comando que nos dará la versión de @angular-cli:

`C:\> ng --version`

![cli version](https://i.ibb.co/WGdCkMH/cliversion.png)

En este punto podemos ya generar nuestra primera aplicación con CLI:

    C:\> ng new miapp --routing
    
La estructura de carpetas que tendremos, será la siguiente:

![estructura aplicación](https://i.ibb.co/nB5QB5P/treeangular.png)

Hay algunos modificadores que podemos utilizar a la hora de generar la aplicación. Personalmente suelo utilizar los siguientes tres modificadores :

 - **routing**:  Genera de manera automática el modulo ***routing.module.ts*** ​ . Este modulo sirve para enrutar las diferentes páginas de nuestra aplicación, por lo que es algo  prácticamente imprescindible en nuestra app.
 
 - **skip-tests**: -   Evita que se generen los archivos de test que se generan por defecto para cada componente.

- **prefix** *nombre-nuevo-prefijo*: ​Por defecto el prefijo de la aplicación es **app**, es decir cualquier componente generado mediante cli tendrá como prefijo **app**-nombre-component​e.​​

       C:\> ng new nombreApp --routing --skip-tests --prefix ex


       




