# Práctica 13

## Instalación de WordPress con Bitnami

- Creamos una máquina de Ubuntu Server en AWS con, mínimo, 2GB de RAM.

- En la máquina ejecutamos el script install-bitnami.sh, el cual lleva los siguientes comandos:

    - Primero actualizamos los paquetes:

        ```
        apt update -y
        apt upgrade -y (opcional)
        ```

    - Descargamos el instalador desde la página oficial de Bitnami:

        `wget https://bitnami.com/redirect/to/1448613/bitnami-wordpress-5.7.1-0-linux-x64-installer.run`

    - Damos permisos de ejecución al instalador:

        `chmod a+x bitnami-wordpress-5.7.1-0-linux-x64-installer.run`

    - Instalamos los paquetes de libreria necesarios:

        `apt-get install libncurses5 -y`

    - Por último, ejecutamos el instalador:

        `./bitnami-wordpress-5.7.1-0-linux-x64-installer.run`