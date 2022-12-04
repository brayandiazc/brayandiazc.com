---
layout: "../../layouts/BlogPost.astro"
title: "Configuracion WSL y Ubuntu 🖥️"
subtitle: "def initial_config(wsl, ubuntu)"
description: "Configuraciòn inicial de WSL y Ubuntu para un entorno de desarrollo"
pubDate: "Dec 8 2022"
heroImage: "/images/blog/configuracion-inicial-wsl-ubuntu.jpg"
imageSource: "unplash.com"
imageUrl: "https://unsplash.com/es/fotos/NLSXFjl_nhc?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink"
---

Despues de instalar WSL o Ubuntu, es necesario realizar una serie de configuraciones para tener un entorno de desarrollo optimo. Para ello debemos abrir una terminal de Ubuntu.

Debemos tener en cuenta que el comando `sudo` nos permite ejecutar comandos como administrador. En este caso, nos permite instalar paquetes.

Para instalar paquetes en Ubuntu, se utiliza el comando `apt-get` o el comando `apt`.

```bash
sudo apt-get install <package>
```

Al ejecutar los comandos para instalar paquetes, nos pedira la contraseña de nuestro usuario. Esta contraseña es la misma que utilizamos para iniciar sesion en Ubuntu.

tambien nos pedira confirmar la instalacion de los paquetes. Para ello, debemos presionar la tecla `y` y luego presionar la tecla `enter`.

## Instalación de paquetes

Actualizamos la lista de paquetes y dependencias:

```bash
sudo apt update && sudo apt upgrade && sudo apt full-upgrade
```

Limpiamos el sistema de paquetes innecesarios:

```bash
sudo apt clean && sudo apt autoclean && sudo apt autoremove
```

Reconocer particiones:

```bash
sudo apt-get install exfat-fuse hfsplus hfsutils ntfs-3g
```

Reconocer smartphones:

```bash
sudo apt-get install mtp-tools ipheth-utils ideviceinstaller ifuse
```

Manejar archivos comprimidos:

```bash
sudo apt-get install p7zip-full p7zip-rar rar unrar
```

Librerias esenciales para programar:

```bash
sudo apt install git-core build-essential curl wget openssl libssl-dev libreadline-dev dirmngr zlib1g-dev libmagickwand-dev imagemagick-6.q16 libffi-dev libpq-dev cmake libwebp-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev software-properties-common libcurl4-openssl-dev
```

Estas librerias ☝️ son necesarias para instalar Ruby, NodeJS, Python, etc.
