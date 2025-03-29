<!--
To README zostało automatycznie wygenerowane przez <https://github.com/YunoHost/apps/tree/master/tools/readme_generator>
Nie powinno być ono edytowane ręcznie.
-->

# OliveTin dla YunoHost

[![Poziom integracji](https://apps.yunohost.org/badge/integration/olivetin)](https://ci-apps.yunohost.org/ci/apps/olivetin/)
![Status działania](https://apps.yunohost.org/badge/state/olivetin)
![Status utrzymania](https://apps.yunohost.org/badge/maintained/olivetin)

[![Zainstaluj OliveTin z YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=olivetin)

*[Przeczytaj plik README w innym języku.](./ALL_README.md)*

> *Ta aplikacja pozwala na szybką i prostą instalację OliveTin na serwerze YunoHost.*  
> *Jeżeli nie masz YunoHost zapoznaj się z [poradnikiem](https://yunohost.org/install) instalacji.*

## Przegląd

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


**Dostarczona wersja:** 2025.3.28~ynh1

## Zrzuty ekranu

![Zrzut ekranu z OliveTin](./doc/screenshots/screenshotDesktop.png)

## Dokumentacja i zasoby

- Oficjalna strona aplikacji: <https://www.olivetin.app>
- Oficjalna dokumentacja dla administratora: <https://docs.olivetin.app>
- Repozytorium z kodem źródłowym: <https://github.com/OliveTin/OliveTin>
- Sklep YunoHost: <https://apps.yunohost.org/app/olivetin>
- Zgłaszanie błędów: <https://github.com/YunoHost-Apps/olivetin_ynh/issues>

## Informacje od twórców

Wyślij swój pull request do [gałęzi `testing`](https://github.com/YunoHost-Apps/olivetin_ynh/tree/testing).

Aby wypróbować gałąź `testing` postępuj zgodnie z instrukcjami:

```bash
sudo yunohost app install https://github.com/YunoHost-Apps/olivetin_ynh/tree/testing --debug
lub
sudo yunohost app upgrade olivetin -u https://github.com/YunoHost-Apps/olivetin_ynh/tree/testing --debug
```

**Więcej informacji o tworzeniu paczek aplikacji:** <https://yunohost.org/packaging_apps>
