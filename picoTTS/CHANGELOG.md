## 1.4.0 - 2021-04-02

*  Use gcr.mirrors.ustc.edu.cn/home-assistant for base images


## 1.3.2 - 2021-03-17

*  Specifiy own S6 entrypoint, don't rely on the base image.
*  Updated git to `2.30.2-r0`
*  Updated python3 to `3.8.8-r0`


## 1.3.1 - 2021-03-04

*  Updated git to `2.30.1-r0`
*  Updated python3 to `3.8.7-r1`


## 1.3.0 - 2021-01-30

*  Updated alpine image to `3.13`
*  Updated git to `2.30.0-r0`
*  Updated g++ to `10.2.1_pre1-r3`
*  Updated autoconf to `2.69-r3`
*  Updated popt/popt-dev to `1.18-r0`
*  Updated automake to `1.16.3-r0`
*  Updated python3 to `3.8.7-r0`
*  Use Jemalloc for better memory handling


## 1.2.0 - 2020-10-21

*  Icon and Logo
*  change startup to `application` level


## 1.1.0 - 2020-10-16

*  Update alpine to `3.12`
*  Update git to `2.26.2-r0`
*  Update make to `4.3-r0`
*  Update g++ to `9.3.0-r2`
*  Update automake to `1.16.2-r0`
*  Update python3 to `3.8.5-r0`
*  Use S6-Overlay for execution


## 1.0.9 - 2020-10-06

*  Updated g++ to `9.3.0-r0`
*  Updated python3 to `3.8.2-r1`


## 1.0.8 - 2020-05-22

*  Added docs file
*  Updated Changelog to new format

## 1.0.7 - 2020-04-29

*  Updated git to `2.24.3-r0`


## 1.0.6 - 2020-04-16

*  Updated git to `2.24.2-r0`


## 1.0.5 - 2019-10-15

*  Update g++ to `9.2.0-r4`
*  Update python to `3.8.2-r0`


## 1.0.4 - 2019-10-15

*  Use alpine `3.11`
*  Update dependencies
  * git `2.24.1-r0`
  * g++ `9.2.0-r3`
  * libtool `2.4.6-r7`
  * python3 `1.16-r7`


## 1.0-3 - 2019-10-15

*  Use alpine 3.9 as base image
*  Fixed wrong log command in startup script, which was confusing HASS.io [#20](https://hub.fastgit.org/Poeschl/Hassio-Addons/issues/20).


## 1.0-2 - 2019-10-06

*  ntegration into new build setup


## 1.0-1 - 2019-09-11

*  Fixed wrong voice name decoding


## 1.0 - 2019-08-07

*  Put latest picoTTS inside HASS.io addon
*  Added python wrapper around local picoTTS to use it from outside.
