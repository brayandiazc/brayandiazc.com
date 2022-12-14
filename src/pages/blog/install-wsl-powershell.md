---
layout: "../../layouts/BlogPost.astro"
title: "Instalaci贸n de WSL usando la consola Powershell 馃捇"
subtitle: "require 'Powershell/WSL'"
description: "Usa Linux sin tener que salir de Windows, con WSL. Instalaci贸n por medio de la consola."
pubDate: "Dec 6 2022"
heroImage: "/images/blog/install-wsl-powershell.jpg"
imageSource: "unplash.com"
imageUrl: "https://unsplash.com/es/fotos/xbEVM6oJ1Fs?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink"
---

Durante mucho tiempo, los desarrolladores de software han estado usando Linux como su sistema operativo principal. Sin embargo, para los usuarios de Windows, la 煤nica opci贸n era usar Windows como su sistema operativo principal.

Para poder usar un entorno linux en Windows, se necesitaba una m谩quina virtual con un entorno gr谩fico, que no es la mejor opci贸n para desarrollar software ni para usar el sistema operativo esto debido al alto consumo de recursos por tener que correr dos sistemas operativos, otra opci贸n era usar un dual boot, pero esto no es la mejor opci贸n para los usuarios que no tienen conocimientos de sistemas operativos. Esto ha cambiado con la llegada de **WSL** (Windows Subsystem for Linux).

Aunque WSL no es una soluci贸n completa, es una gran herramienta para los desarrolladores de software que usan Windows como su sistema operativo principal. WSL permite a los usuarios de Windows ejecutar aplicaciones de Linux en Windows sin tener que instalar Linux en una m谩quina virtual o en un disco duro externo o en una partici贸n separada.

## 驴Qu茅 es WSL?

WSL es un sistema operativo de capa intermedia que permite ejecutar aplicaciones de Linux en Windows sin un entorno gr谩fico. Esto significa que puedes usar Linux sin tener que salir de Windows. WSL es una caracter铆stica de Windows 10 y Windows 11 que se lanz贸 en 2016. Desde entonces, ha sido mejorado y actualizado varias veces.

## 驴Qu茅 puedes hacer con WSL?

Puedes usar WSL para ejecutar aplicaciones de Linux en Windows. Esto incluye aplicaciones de l铆nea de comandos, aplicaciones de escritorio y aplicaciones web. Entre las aplicaciones de l铆nea de comandos, puedes usar Git, Node.js, Python, Ruby, PHP, MySQL, MongoDB, etc. Entre las aplicaciones de escritorio, puedes usar aplicaciones como Visual Studio Code, Atom, Sublime Text, etc. Entre las aplicaciones web, puedes usar aplicaciones como WordPress, Laravel, Rails, Django, etc.

### Existen dos versiones de WSL

- **WSL 1** Esta es la versi贸n original de WSL. WSL 1 usa una m谩quina virtual para ejecutar aplicaciones de Linux en Windows. Esto significa que WSL 1 es m谩s lento que WSL 2. Sin embargo, WSL 1 es compatible con m谩s versiones de Linux que WSL 2.

- **WSL 2** Esta es la versi贸n m谩s reciente de WSL. WSL 2 usa un n煤cleo de Linux real para ejecutar aplicaciones de Linux en Windows. Esto significa que WSL 2 es m谩s r谩pido que WSL 1. Sin embargo, WSL 2 solo es compatible con algunas versiones de Linux.

## 驴Qu茅 versiones de Windows son compatibles con WSL?

WSL solo es compatible con Windows 10 y Windows 11. Sin embargo, no todas las versiones de Windows 10 son compatibles con WSL. Para usar WSL, debes tener Windows 10 versi贸n 2004 o posterior. Si no tienes Windows 10 versi贸n 2004 o posterior, puedes actualizar a Windows 10 versi贸n 2004 o posterior. Si tienes Windows 11 instalado, puedes usar WSL sin ning煤n problema.

Puedes comprobar tu versi贸n de Windows 10 en la configuraci贸n de Windows. Para abrir la configuraci贸n de Windows, presiona la tecla de Windows + I. En la configuraci贸n de Windows, haz clic en "Sistema" y luego haz clic en "Informaci贸n". En la p谩gina "Informaci贸n", puedes ver la versi贸n de Windows 10 que tienes instalada.

![Verificar version windows](/images/blogContent/install-wsl-powershell/verificar-version-windows.png)

En mi caso tengo Windows 11, por lo que no tengo ning煤n problema para usar WSL.

## Instalaci贸n de WSL

Para instalar WSL por medio de PowerShell, debes abrir PowerShell como administrador. Para abrir PowerShell como administrador, presiona la tecla de Windows escribe "PowerShell" y luego selecciona la opci贸n "Ejecutar como administrador".

![Powershell](/images/blogContent/install-wsl-powershell/powershell.png)

Despues de abrir powershell como administrador, ejecuta el siguiente comando para instalar WSL:

```powershell
wsl --install
```

Esto es todo lo que necesitas hacer para instalar WSL. Despu茅s de ejecutar el comando, WSL se instalar谩 en tu computadora. Si todo sale bien, ver谩s el siguiente mensaje:

![Instalar WSL](/images/blogContent/install-wsl-powershell/instalacion-wsl.png)

Posteriormente, se te pedir谩 que reinicies tu computadora. Despu茅s de reiniciar tu computadora, WSL estar谩 listo para usar.

## Configuraci贸n de Linux

Para configurar Linux, abre la aplicaci贸n Linux y sigue las instrucciones, te pedir谩 que ingreses un **usuario** y **contrase帽a**. Despu茅s de configurar Linux, puedes usar Linux en Windows.

![Configuraci贸n inicial ubuntu](/images/blogContent/install-wsl-powershell/configuracion-inicial-ubuntu.png)

## Instalaci贸n de aplicaciones de Linux en Windows

Con esto hemos instalado WSL y Linux en Windows. Ahora, podemos instalar aplicaciones de Linux en Windows. Para instalar aplicaciones de Linux en Windows, abre la aplicaci贸n Linux y ejecuta el comando `sudo apt update` para actualizar el 铆ndice de paquetes. Despu茅s de actualizar el 铆ndice de paquetes, ejecuta el comando `sudo apt install <nombre de la aplicaci贸n>` para instalar la aplicaci贸n. Por ejemplo, para instalar Git, ejecuta el comando `sudo apt install git`.
