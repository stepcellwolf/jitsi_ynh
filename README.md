<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Jitsi Meet for YunoHost

[![Integration level](https://dash.yunohost.org/integration/jitsi.svg)](https://dash.yunohost.org/appci/app/jitsi) ![](https://ci-apps.yunohost.org/ci/badges/jitsi.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/jitsi.maintain.svg)  
[![Install Jitsi Meet with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=jitsi)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install Jitsi Meet quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

Jitsi Meet is a libre software (Apache) WebRTC JavaScript app that uses Jitsi Videobridge to provide high quality, secure, and scalable video conferences.


**Shipped version:** 1.0.6155~ynh1

**Demo:** https://meet.jit.si/

## Screenshots

![](./doc/screenshots/screenshot.png)

## Disclaimers / important information

## Important points before installing

1. **Jitsi** requires a dedicated **root domain**, eg. jitsi.domain.tld
2. **Jitsi** requires the ports TCP/4443 and UDP/10000 to be forwarded to your YunoHost (The same way you forwarded 80 (HTTP), 443 (HTTPS), etc... https://yunohost.org/#/isp_box_config)
3. **Jitsi** will stop and disable Metronome XMPP.
4. LDAP authentication is activated, only authenticated users to create new conference rooms. Whenever a new room is about to be created, Jitsi Meet will prompt for a user name and password. After the room is created, others will be able to join from anonymous domain.
5. **Jitsi** is configured for 50 users maximum, this number can be increase going to the Yunohost config panel

## Documentation and resources

* Official app website: https://jitsi.org/
* Official user documentation: https://jitsi.org/user-faq/
* Upstream app code repository: https://github.com/jitsi/jitsi-meet
* YunoHost documentation for this app: https://yunohost.org/app_jitsi
* Report a bug: https://github.com/YunoHost-Apps/jitsi_ynh/issues

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/jitsi_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/jitsi_ynh/tree/testing --debug
or
sudo yunohost app upgrade jitsi -u https://github.com/YunoHost-Apps/jitsi_ynh/tree/testing --debug
```

**More info regarding app packaging:** https://yunohost.org/packaging_apps