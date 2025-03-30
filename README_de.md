<!--
N.B.: Diese README wurde automatisch von <https://github.com/YunoHost/apps/tree/master/tools/readme_generator> generiert.
Sie darf NICHT von Hand bearbeitet werden.
-->

# OliveTin für YunoHost

[![Integrations-Level](https://apps.yunohost.org/badge/integration/olivetin)](https://ci-apps.yunohost.org/ci/apps/olivetin/)
![Funktionsstatus](https://apps.yunohost.org/badge/state/olivetin)
![Wartungsstatus](https://apps.yunohost.org/badge/maintained/olivetin)

[![OliveTin mit YunoHost installieren](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=olivetin)

*[Dieses README in anderen Sprachen lesen.](./ALL_README.md)*

> *Mit diesem Paket können Sie OliveTin schnell und einfach auf einem YunoHost-Server installieren.*  
> *Wenn Sie YunoHost nicht haben, lesen Sie bitte [die Anleitung](https://yunohost.org/install), um zu erfahren, wie Sie es installieren.*

## Übersicht

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


**Ausgelieferte Version:** 2025.3.28~ynh1

## Bildschirmfotos

![Bildschirmfotos von OliveTin](./doc/screenshots/screenshotDesktop.png)

## Dokumentation und Ressourcen

- Offizielle Website der App: <https://www.olivetin.app>
- Offizielle Verwaltungsdokumentation: <https://docs.olivetin.app>
- Upstream App Repository: <https://github.com/OliveTin/OliveTin>
- YunoHost-Shop: <https://apps.yunohost.org/app/olivetin>
- Einen Fehler melden: <https://github.com/YunoHost-Apps/olivetin_ynh/issues>

## Entwicklerinformationen

Bitte senden Sie Ihren Pull-Request an den [`testing` branch](https://github.com/YunoHost-Apps/olivetin_ynh/tree/testing).

Um den `testing` Branch auszuprobieren, gehen Sie bitte wie folgt vor:

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/olivetin_ynh/tree/testing --debug
oder
sudo yunohost app upgrade olivetin -u https://github.com/YunoHost-Apps/olivetin_ynh/tree/testing --debug
```

**Weitere Informationen zur App-Paketierung:** <https://yunohost.org/packaging_apps>
