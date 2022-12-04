---
layout: "../../layouts/BlogPost.astro"
title: "Instalación de WSL usando la consola Powershell 💻"
subtitle: "require 'Powershell/WSL'"
description: "Usa Linux sin tener que salir de Windows, con WSL. Instalación por medio de la consola."
pubDate: "Dec 6 2022"
heroImage: "/images/blog/install-wsl-powershell.jpg"
imageSource: "unplash.com"
imageUrl: "https://unsplash.com/es/fotos/4Mw7nkQDByk?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink"
---

Durante mucho tiempo, los desarrolladores de software han estado usando Linux como su sistema operativo principal. Sin embargo, para los usuarios de Windows, la única opción era usar Windows como su sistema operativo principal.

Para poder usar un entorno linux en Windows, se necesitaba una máquina virtual con un entorno gráfico, que no es la mejor opción para desarrollar software ni para usar el sistema operativo esto debido al alto consumo de recursos por tener que correr dos sistemas operativos, otra opción era usar un dual boot, pero esto no es la mejor opción para los usuarios que no tienen conocimientos de sistemas operativos. Esto ha cambiado con la llegada de **WSL** (Windows Subsystem for Linux).

Aunque WSL no es una solución completa, es una gran herramienta para los desarrolladores de software que usan Windows como su sistema operativo principal. WSL permite a los usuarios de Windows ejecutar aplicaciones de Linux en Windows sin tener que instalar Linux en una máquina virtual o en un disco duro externo o en una partición separada.

## ¿Qué es WSL?

WSL es un sistema operativo de capa intermedia que permite ejecutar aplicaciones de Linux en Windows sin un entorno gráfico. Esto significa que puedes usar Linux sin tener que salir de Windows. WSL es una característica de Windows 10 y Windows 11 que se lanzó en 2016. Desde entonces, ha sido mejorado y actualizado varias veces.

## ¿Qué puedes hacer con WSL?

Puedes usar WSL para ejecutar aplicaciones de Linux en Windows. Esto incluye aplicaciones de línea de comandos, aplicaciones de escritorio y aplicaciones web. Entre las aplicaciones de línea de comandos, puedes usar Git, Node.js, Python, Ruby, PHP, MySQL, MongoDB, etc. Entre las aplicaciones de escritorio, puedes usar aplicaciones como Visual Studio Code, Atom, Sublime Text, etc. Entre las aplicaciones web, puedes usar aplicaciones como WordPress, Laravel, Rails, Django, etc.

### Existen dos versiones de WSL

- **WSL 1** Esta es la versión original de WSL. WSL 1 usa una máquina virtual para ejecutar aplicaciones de Linux en Windows. Esto significa que WSL 1 es más lento que WSL 2. Sin embargo, WSL 1 es compatible con más versiones de Linux que WSL 2.

- **WSL 2** Esta es la versión más reciente de WSL. WSL 2 usa un núcleo de Linux real para ejecutar aplicaciones de Linux en Windows. Esto significa que WSL 2 es más rápido que WSL 1. Sin embargo, WSL 2 solo es compatible con algunas versiones de Linux.

## ¿Qué versiones de Windows son compatibles con WSL?

WSL solo es compatible con Windows 10 y Windows 11. Sin embargo, no todas las versiones de Windows 10 son compatibles con WSL. Para usar WSL, debes tener Windows 10 versión 2004 o posterior. Si no tienes Windows 10 versión 2004 o posterior, puedes actualizar a Windows 10 versión 2004 o posterior. Si tienes Windows 11 instalado, puedes usar WSL sin ningún problema.

Puedes comprobar tu versión de Windows 10 en la configuración de Windows. Para abrir la configuración de Windows, presiona la tecla de Windows + I. En la configuración de Windows, haz clic en "Sistema" y luego haz clic en "Información". En la página "Información", puedes ver la versión de Windows 10 que tienes instalada.

![Verificar version windows](/images/blogContent/install-wsl-powershell/verificar-version-windows.png)

En mi caso tengo Windows 11, por lo que no tengo ningún problema para usar WSL.

## Instalación de WSL

Para instalar WSL por medio de PowerShell, debes abrir PowerShell como administrador. Para abrir PowerShell como administrador, presiona la tecla de Windows escribe "PowerShell" y luego selecciona la opción "Ejecutar como administrador".

![Powershell](/images/blogContent/install-wsl-powershell/powershell.png)

Despues de abrir powershell como administrador, ejecuta el siguiente comando para instalar WSL:

```powershell
wsl --install
```

Esto es todo lo que necesitas hacer para instalar WSL. Después de ejecutar el comando, WSL se instalará en tu computadora. Si todo sale bien, verás el siguiente mensaje:

![Instalar WSL](/images/blogContent/install-wsl-powershell/instalacion-wsl.png)

Posteriormente, se te pedirá que reinicies tu computadora. Después de reiniciar tu computadora, WSL estará listo para usar.

## Configuración de Linux

Para configurar Linux, abre la aplicación Linux y sigue las instrucciones, te pedirá que ingreses un **usuario** y **contraseña**. Después de configurar Linux, puedes usar Linux en Windows.

![Configuración inicial ubuntu](/images/blogContent/install-wsl-powershell/configuracion-inicial-ubuntu.png)

## Instalación de aplicaciones de Linux en Windows

Con esto hemos instalado WSL y Linux en Windows. Ahora, podemos instalar aplicaciones de Linux en Windows. Para instalar aplicaciones de Linux en Windows, abre la aplicación Linux y ejecuta el comando `sudo apt update` para actualizar el índice de paquetes. Después de actualizar el índice de paquetes, ejecuta el comando `sudo apt install <nombre de la aplicación>` para instalar la aplicación. Por ejemplo, para instalar Git, ejecuta el comando `sudo apt install git`.
