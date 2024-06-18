<!--
Este archivo README esta generado automaticamente<https://github.com/YunoHost/apps/tree/master/tools/readme_generator>
No se debe editar a mano.
-->

# OliveTin para Yunohost

[![Nivel de integración](https://dash.yunohost.org/integration/olivetin.svg)](https://dash.yunohost.org/appci/app/olivetin) ![Estado funcional](https://ci-apps.yunohost.org/ci/badges/olivetin.status.svg) ![Estado En Mantención](https://ci-apps.yunohost.org/ci/badges/olivetin.maintain.svg)

[![Instalar OliveTin con Yunhost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=olivetin)

*[Leer este README en otros idiomas.](./ALL_README.md)*

> *Este paquete le permite instalarOliveTin rapidamente y simplement en un servidor YunoHost.*  
> *Si no tiene YunoHost, visita [the guide](https://yunohost.org/install) para aprender como instalarla.*

## Descripción general

OliveTin gives safe and simple access to predefined shell commands from a web interface.

## Use cases
###  Safely give access to commands, for less technical people

- Give your family a button to `systemctl restart jellyfin`
- Give junior admins a simple web form with dropdowns, to start your custom script like `backupScript.sh --folder {{ customerName }}`
- Enable SSH access to the server for the next 20 mins `firewall-cmd --add-service ssh --timeout 20m`

### Simplify complex commands, make them accessible and repeatable

- Expose complex commands on touchscreen tablets stuck on walls around your house. `wake-on-lan aa:bb:cc:11:22:33`
- Run long running on your servers from your cell phone. `apt upgrade -y`

## Features

- Responsive, touch-friendly UI - great for tablets and mobile
- Super simple config in YAML - because if it’s not YAML now-a-days, it’s not "cloud native" :-)
- Dark mode - for those of you that roll that way.
- Accessible - passes all the accessibility checks in Firefox, and issues with accessibility are taken seriously.
- Container - available for quickly testing and getting it up and running, great for the selfhosted community.
- Integrate with anything - OliveTin just runs Linux shell commands, so theoretially you could integrate with a bunch of stuff just by using curl, ping, etc. However, writing your own shell scripts is a reat way to extend OliveTin.
- Lightweight on resources - uses only a few MB of RAM and barely any CPU. Written in Go, with a web interface written as a modern, responsive, Single Page App that uses the REST/gRPC API.
- Good amount of unit tests and style checks - helps potential contributors be consistent, and helps with maintainability.


**Versión actual:** 2023.02.16~ynh1

## Capturas

![Captura de OliveTin](./doc/screenshots/example.jpg)

## Documentaciones y recursos

- Sitio web oficial: <https://www.olivetin.app>
- Documentación administrador oficial: <https://docs.olivetin.app>
- Repositorio del código fuente oficial de la aplicación : <https://github.com/OliveTin/OliveTin>
- Catálogo YunoHost: <https://apps.yunohost.org/app/olivetin>
- Reportar un error: <https://github.com/YunoHost-Apps/olivetin_ynh/issues>

## Información para desarrolladores

Por favor enviar sus correcciones a la [`branch testing`](https://github.com/YunoHost-Apps/olivetin_ynh/tree/testing

Para probar la rama `testing`, sigue asÍ:

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/olivetin_ynh/tree/testing --debug
o
sudo yunohost app upgrade olivetin -u https://github.com/YunoHost-Apps/olivetin_ynh/tree/testing --debug
```

**Mas informaciones sobre el empaquetado de aplicaciones:** <https://yunohost.org/packaging_apps>
