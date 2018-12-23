# GOOGLEDEVICES [![Build Status][travis_status]][travis] [![PyPI version][pypi_badge]][pypi]

[**HOME**][home] | [PLATFORMS][platforms] | [CLASSES][classes] | [METHODS][methods] | [FUNCTIONS][functions] | [CLI][cli]

This Python package is based of the works of [rithvikvibhu/GHLocalApi][GHLocalApi]

## HOME

### Installation

```bash
pip install googledevices
```

This package also comes with a CLI.  

```bash
Usage: googledevices [OPTIONS] COMMAND [ARGS]...

Options:
  --help  Show this message and exit.

Commands:
  alarm-volume           Get or set alarm volume.
  debug                  Get debug information.
  device-info            Get information about a Google device on your...
  get-all-devices        Get information about all devices on your network.
  get-bluetooth-devices  Get bluetooth devices from a unit.
  googlewifi-clients     Get devices from google wifi.
  googlewifi-info        Get information about google wifi.
  info                   Get information about this package.
  reboot                 Reboot a Google device.
  scan-network           Scan the entire subnet for Google devices.
```

Sample usage of the CLI:

```bash
username@hostname:~$ googledevices scan-network
[
    {
        "assistant": false,
        "bluetooth": false,
        "host": "192.168.2.136",
        "model": "Chromecast Ultra",
        "name": "ChromeCast ULTRA"
    },
    {
        "assistant": false,
        "bluetooth": false,
        "host": "192.168.2.188",
        "model": "Chromecast",
        "name": "Chrome Cast"
    },
    {
        "assistant": true,
        "bluetooth": true,
        "host": "192.168.2.234",
        "model": "Google Home Mini",
        "name": "Living Room"
    }
]
```

### Maintainers

- [ludeeus][ludeeus]
- [eliseomartelli][eliseomartelli]

#### Notice

_This is not affiliated, associated, authorized, endorsed by, or in any way officially connected with [Alphabet][alphabet], or any of its subsidiaries or its affiliates. The name "Google" as well as related names, marks, emblems and images are registered trademarks of [Alphabet][alphabet]._


## Contributing

1. [Check for open features/bugs][issues]
  or [initiate a discussion on one][issues-new].
2. [Fork the repository][fork].
3. Install the dev environment: `make init`.
4. Enter the virtual environment: `pipenv shell`
5. Code your new feature or bug fix.
6. Run `make lint` and make sure the score still is `10.00/10`
7. Submit a [pull request][pull-request]!


<!-- links -->
[alphabet]: https://abc.xyz/
[commands]: https://github.com/ludeeus/googledevices/tree/master/googledevices/cli/commands
[eliseomartelli]: https://github.com/eliseomartelli
[fork]: https://github.com/ludeeus/googledevices/fork
[GHLocalApi]: https://github.com/rithvikvibhu/GHLocalApi
[issues]: https://github.com/ludeeus/googledevices/issues
[issues-new]: https://github.com/ludeeus/googledevices/issues/new
[ludeeus]: https://github.com/ludeeus
[pull-request]: https://github.com/ludeeus/googledevices/compare

<!-- menu -->
[travis]: https://travis-ci.com/ludeeus/googledevices
[travis_status]: https://travis-ci.com/ludeeus/googledevices.svg?branch=master
[pypi]:https://pypi.org/project/googledevices/
[pypi_badge]: https://badge.fury.io/py/googledevices.svg
[home]: https://ludeeus.github.io/ROOT/index.md
[platforms]: https://ludeeus.github.io/ROOT/platfroms.md
[classes]: https://ludeeus.github.io/ROOT/classes.md
[methods]: https://ludeeus.github.io/ROOT/methods.md
[functions]: https://ludeeus.github.io/ROOT/functions.md
[cli]: https://ludeeus.github.io/ROOT/cli.md