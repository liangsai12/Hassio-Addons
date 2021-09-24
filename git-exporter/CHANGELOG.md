## 1.10.1 - 2021-06-03

*  Add secrets corner case docs for secrets containing special regex chars. (thanks @fliphess)


## 1.10.0 - 2021-05-08

*  Don't encode GitHub Tokens
*  Updated python3 to `3.8.10-r0`


## 1.9.0 - 2021-04-02

*  Use gcr.mirrors.ustc.edu.cn/home-assistant for base images


## 1.8.0 - 2021-03-30

*  URL encode git password to support special chars (see #219)
*  Updated git to `2.30.2-r0`
*  Updated python3 to `3.8.8-r0`


## 1.7.1 - 2021-03-04

*  Updated git to `2.30.1-r0`
*  Updated python3 to `3.8.7-r1`


## 1.7.0 - 2021-01-30

*  Updated to alpine `3.13`
*  Updated git to `2.30.0-r0`
*  Updated rsync to `3.2.3-r1`
*  Updated grep to `3.6-r0`
*  Updated python3 to `3.8.7-r0`
*  Updated py3-pip to `20.3.4-r0`
*  Updated findutils to `4.8.0-r0`
*  Use Jemalloc for better memory handling


## 1.6.0 - 2021-01-06

*  Add dummy mac and ip adresses as allowed
*  Exclude also all Node-Red backup files


## 1.5.0 - 2020-12-29

*  Fixed addon config export (#135), thanks @LiJu09

## 1.4.4 - 2020-10-22

*  Disable S6-Overlay Init


## 1.4.3 - 2020-10-06

*  Updated python3 to `3.8.5-r0`


## 1.4.2 - 2020-06-25

*  Updated to alpine `3.12`
*  Updated git to `2.26.2-r0`
*  Updated make to `4.3-r0`
*  Updated rsync to `3.1.3-r3`
*  Updated grep to `3.4-r0`
*  Updated sed to `4.8-r0`
*  Updated python3 to `3.8.3-r0`
*  Updated py3-pip to `20.1.1-re0`
*  Added more default ignore patterns


## 1.4.1 - 2020-05-22

*  Updated Changelog to new format


## 1.4.0 - 2020-05-20

*  Export addon repositories
*  Changed config documentation
*  Add Node-Red check
*  Add commiter email option


## 1.3.2 - 2020-04-29

*  Updated git to `2.24.3-r0`


## 1.3.1 - 2020-04-16

*  Updated git to `2.24.2-r0`


## 1.3.0 - 2020-04-06

*  Add export support for node-red


## 1.2.1 - 2020-03-30

*  Add findutils at version `4.7.0-r0`
*  Fixed lovelace export
*  Get the addon information from bashio instead of self-requesting
*  Removed `curl`


## 1.2.0 - 2020-03-29

*  Changed json2yaml conversion to own little script
*  Updated py3-yaml ot `5.3.1-r0`
*  Fixed permanent dry_run bug


## 1.1.0 - 2020-03-18

*  Dry run toogle to just display the changes.
*  Adjusted to the multiple lovelace interfaces
*  Updated to python `3.8.2-r0`


## 1.0 - 2020-02-21

*  Started git exporter addon with basic git push functionality
*  Added excludes in config
*  Lovelace exports
*  Addons config exports
*  ESPHome exports
*  Configurable Commit message
*  Configurable exports

