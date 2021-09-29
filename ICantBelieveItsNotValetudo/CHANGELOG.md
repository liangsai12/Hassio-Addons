## 3.4.1 - 2021-07-27

*  Added port of mqtt broker to schema validaton
*  Update alpine to `3.14`
*  Update git to `2.32.0-r0`
*  Update npm to `7.17.0-r0`
*  Update pango/pango-dev to `1.48.5-r0`
*  Update cairo/cairo-dev to `1.16.0-r3`
*  Updated python3 to `3.9.5-r1`

## 3.4.0 - 2021-06-20

*  Updated ICantBelieveItsNotValetudo to latest release `2021.6.0` (thanks @ishioni)
*  Updated python3 to `3.8.10-r0`

## 3.3.1 - 2021-05-03

*  Updated ICantBelieveItsNotValetudo default mqtt path, (@shalak)


## 3.3.0 - 2021-04-25

*  Updated ICantBelieveItsNotValetudo to latest release `2021.4.0`
*  Updated libjpeg-turbo/libjpeg-turbo-dev to `2.1.0-r0`
*  Updated npm to `14.16.1-r1`


## 3.2.0 - 2021-04-02

*  Updated ICantBelieveItsNotValetudo to latest release `2021.3.1`
*  Bring back the png image via webserver.


## 3.1.0 - 2021-04-02

*  Use ghcr.io/home-assistant for base images


## 3.0.1 - 2021-03-17

*  Specifiy own S6 entrypoint, don't rely on the base image.
*  Add optional `segments` color setting
*  Update git to `2.30.2-r0`
*  Updated python3 to `3.8.8-r0`


## 3.0.0 - 2021-02-27

*  Updated ICantBelieveItsNotValetudo to latest commit `73a7965` to make it fully compatible with Valetudo > 2021.02.1
*  Updated npm to `14.16.0-r0`
*  Removed `homeassistantMapHack` notice


## 2.8.1 - 2021-02-20

*  Updated python3 to `3.8.7-r1`
*  Changed the addon configuration to the current configuration of ICantBelieveItsNotValetudo (removing under/overlay images and cropping)
*  Add `homeassistantMapHack` notice
*  Removed `/share` mount


## 2.8.0 - 2021-02-18

*  Updated ICantBelieveItsNotValetudo to latest commit `74b6c33`
*  Updated npm to `14.15.5-r0`
*  Unspecify version of pkgconf
*  Removed webserver since [no image is served anymore](https://hub.fastgit.org/Hypfer/ICantBelieveItsNotValetudo/commit/54cc0d96a6c03ee4dc92b86e533c0cd3999a7068#diff-b335630551682c19a781afebcf4d07bf978fb1f8ac04c6bf87428ed5106870f5L14)
*  Removed ingress since not needed anymore, since nothing to serve

###  Note 

* No image will be served to the side panel anymore. The map is only available as mqtt camera.


## 2.7.0 - 2021-02-15

*  Allow also anonymous access in mqtt broker url
*  Updated pango to `1.48.2-r0`


## 2.6.1 - 2021-02-10

*  Updated git to `2.30.1-r0`


## 2.6.0 - 2021-01-30

*  Updated alpine image to `3.13`
*  Updated git to `2.30.0-r0`
*  Updated npm to `14.15.4-r0`
*  Updated python3 to `3.8.7-r0`
*  Updated pkgconf to `1.7.3-r0`
*  Updated pango/pango-dev to `1.48.1-r0`
*  Updated libjpeg-turbo/libjpeg-turbo-dev to `2.0.6-r0`
*  Use Jemalloc for better memory handling


## 2.5.0 - 2020-12-14

*  Include small webserver to center the floorplan and apply the HA theme.
*  Updated ICantBelieveItsNotValetudo to latest commit `bd687c1`


## 2.4.0 - 2020-11-28

*  Updated ICantBelieveItsNotValetudo to latest commit `4b4a62c`


## 2.3.0 - 2020-10-23

*  Updated ICantBelieveItsNotValetudo to latest commit `67f86e2`

###  Breaking Change 

* Colors are only supported as hex values. See [Colors](https://hub.fastgit.org/Hypfer/ICantBelieveItsNotValetudo#new-map-colors)
* Colors are not optional anymore, they will be set to the defaults if not existing.

## 2.2.2 - 2020-10-22

*  Start as `application` startup type

## 2.2.1 - 2020-10-06

*  Updated npm to `12.18.4-r0`

## 2.2.0 - 2020-07-29

*  Updated ICantBelieveItsNotValetudo to latest commit `30945f9` to use the new map data format
*  Updated alpine image to `3.12`
*  Updated git to `2.26.2-r0`
*  Updated npm to `12.17.0-r0`
*  Change build system to two-staged system for compiling needed npm packages outside of the running image
*  Use S6 system

## 2.1.0 - 2020-05-29

*   Updated ICantBelieveItsNotValetudo to latest commit `9bcfc25`

## 2.0.3 - 2020-05-22

*  Updated Changelog to new format

## 2.0.2 - 2020-04-29

*  Updated git to `2.24.3-r0`

## 2.0.1 - 2020-04-16

*  Updated git to `2.24.2-r0`

## 2.0.0 - 2020-02-27

*  Updated ICantBelieveItsNotValetudo to latest commit `3cf4f8a`
*  Adjusted to new config structure (__Make sure to migrate your existing config!__)

## 1.0.0 - 2020-02-07

*  Own versioning for changes. Start with `1.0.0`
*  Updated Dependencies:
  * alpine `3.11`
  * git `2.24.1-r0`
  * npm `12.15.0-r1`

## 0.2.0-5 - 2019-11-06

*  Added schema for optional cropping parameters

## 0.2.0-4 - 2019-10-19

*  Switch to current master instead of latest version (thanks @Nickerchen)

## 0.2.0-3 - 2019-10-15

*  Use alpine 3.9 as base image

## 0.2.0-2 - 2019-10-06

*  Integration into new build setup

## 0.2.0-1 - 2019-09-02

*  Added HASS.io Ingress feature (#6)
*  Ingress is now the default access method

## 0.2.0 - 2019-08-14

*  SSL Mapping on HASS.io
*  Add ICantBelieveItsNotValetudo Version 0.2.0 in its basic form
*  Added plugin to pre-built ones
*  Fixed MQTT config setting
