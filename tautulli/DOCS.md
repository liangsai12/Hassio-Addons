# Home Assistant Community Add-on: Tautulli

Tautulli is an application that you can run alongside your Plex Media Server
to monitor activity, and track various statistics.
Most importantly, these statistics include what has been watched,
who watched it, when and where they watched it, and how it was watched.
All statistics are presented in a nice and clean interface
with many tables and graphs,
which makes it easy to brag about your server to everyone else.

## Installation

The installation of this add-on is pretty straightforward and not different in
comparison to installing any other Home Assistant add-on.

1. Search for the "Tautulli" add-on in the Supervisor add-on store
   and install it.
1. Start the "Tautulli" add-on
1. Check the logs of the "Tautulli" add-on to see if everything went well.
1. Click "OPEN WEB UI" to open the Tautulli website and follow the wizard.

**NOTE**: Starting the add-on might take a couple of minutes (especially the
first time starting the add-on).

## Configuration

**Note**: _Remember to restart the add-on when the configuration is changed._

Example add-on configuration:

```yaml
log_level: info
username: MarryPoppins
password: Supercalifragilisticexpialidocious
ssl: true
certfile: fullchain.pem
keyfile: privkey.pem
```

**Note**: _This is just an example, don't copy and past it! Create your own!_

### Option: `log_level`

The `log_level` option controls the level of log output by the addon and can
be changed to be more or less verbose, which might be useful when you are
dealing with an unknown issue. Possible values are:

- `trace`: Show every detail, like all called internal functions.
- `debug`: Shows detailed debug information.
- `info`: Normal (usually) interesting events.
- `warning`: Exceptional occurrences that are not errors.
- `error`: Runtime errors that do not require immediate action.
- `fatal`: Something went terribly wrong. Add-on becomes unusable.

Please note that each level automatically includes log messages from a
more severe level, e.g., `debug` also shows `info` messages. By default,
the `log_level` is set to `info`, which is the recommended setting unless
you are troubleshooting.

### Option: `username`

Username for authenticating with the Tautulli interface.

Setting a username/password can be added as an extra line of defense,
to prevent users from using your installation for themselves.

This option is HIGHLY recommended in case you expose this add-on to the outside
world.

### Option: `password`

Password for authenticating with Tautulli interface.

### Option: `ssl`

Enables/Disables SSL (HTTPS) on the web interface of Tautulli. Set it `true`
to enable it, `false` otherwise.

### Option: `certfile`

The certificate file to use for SSL.

**Note**: _The file MUST be stored in `/ssl/`, which is the default_

### Option: `keyfile`

The private key file to use for SSL.

**Note**: _The file MUST be stored in `/ssl/`, which is the default_

### Option: `leave_front_door_open`

Adding this option to the add-on configuration allows you to disable
authentication on the add-on by setting it to `true` and leaving the
username and password empty.

**Note**: _We STRONGLY suggest, not to use this, even if this add-on is
only exposed to your internal network. USE AT YOUR OWN RISK!_

## Embedding into Home Assistant

It is possible to embed Tautulli directly into Home Assistant, allowing you to
access your Tautulli through the Home Assistant frontend.

Home Assistant provides the `panel_iframe` integration, for these purposes.

Example configuration:

```yaml
panel_iframe:
  tautulli:
    title: Tautulli
    icon: mdi:filmstrip
    url: http://addres.to.your.home.assistant:8181
```

## Use an existing database

**NB!: This is considered advanced usage.**

If you want to import an existing Tautulli database to this addon, you first
need to extract the `tautulli.db` file from your existing installation.
Place this file in this directory `/share/tautulli`, you can use samba,
Cloud9 or any other method to move it there.
You need to restart the add-on for it to start using this database.
_if the directory `/share/tautulli` does not exist you need to create it._

## Changelog & Releases

This repository keeps a change log using [GitHub's releases][releases]
functionality.

Releases are based on [Semantic Versioning][semver], and use the format
of `MAJOR.MINOR.PATCH`. In a nutshell, the version will be incremented
based on the following:

- `MAJOR`: Incompatible or major changes.
- `MINOR`: Backwards-compatible new features and enhancements.
- `PATCH`: Backwards-compatible bugfixes and package updates.

## Support

Got questions?

You have several options to get them answered:

- The [Home Assistant Community Add-ons Discord chat server][discord] for add-on
  support and feature requests.
- The [Home Assistant Discord chat server][discord-ha] for general Home
  Assistant discussions and questions.
- The Home Assistant [Community Forum][forum].
- Join the [Reddit subreddit][reddit] in [/r/homeassistant][reddit]

You could also [open an issue here][issue] GitHub.

## Authors & contributors

The original setup of this repository is by [Joakim Sorensen][ludeeus].

For a full list of all authors and contributors,
check [the contributor's page][contributors].

## License

MIT License

Copyright (c) 2018-2021 Joakim Sorensen

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[contributors]: https://hub.fastgit.org/hassio-addons/addon-tautulli/graphs/contributors
[discord-ha]: https://discord.gg/c5DvZ4e
[discord]: https://discord.me/hassioaddons
[forum]: https://community.home-assistant.io/t/home-assistant-community-add-on-tautulli/68745?u=ludeeus
[issue]: https://hub.fastgit.org/hassio-addons/addon-tautulli/issues
[ludeeus]: https://hub.fastgit.org/ludeeus
[reddit]: https://reddit.com/r/homeassistant
[releases]: https://hub.fastgit.org/hassio-addons/addon-tautulli/releases
[semver]: http://semver.org/spec/v2.0.0.htm