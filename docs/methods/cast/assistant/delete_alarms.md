[![Build Status][travis_status]][travis] [![PyPI version][pypi_badge]][pypi] _Get information from, and control various Google devices._

***

[HOME][home] | [PLATFORMS][platforms] | [CLASSES][classes] | [**METHODS**][methods] | [FUNCTIONS][functions] | [CLI][cli]

***

## Cast - Assistant - `delete_alarms`

This takes one required parameter.  
This **needs** to be formated like this:

```json
[ "timer\/xxx", "alarm\/xxx" ]
```

Sample usage:

```python
from googledevices.api.connect import Cast
from googledevices.helpers import gdh_session, gdh_loop, gdh_sleep
from googledevices.utils.convert import format_json

CAST_HOST = '192.168.2.241'
LOOP = gdh_loop()

async def sample():
    """Sample usage."""
    async with gdh_session() as session:
        print("Testing Cast - Assistant - delete_alarms")
        test_class = await Cast(TEST_HOST_CAST, LOOP, session).assistant()
        data = [ "timer\/984", "alarm\/234" ]
        test = await test_class.delete_alarms(data)
        print(format_json(test))
LOOP.run_until_complete(sample())
```

<!-- menu -->
[travis]: https://travis-ci.com/ludeeus/googledevices
[travis_status]: https://travis-ci.com/ludeeus/googledevices.svg?branch=master
[pypi]:https://pypi.org/project/googledevices/
[pypi_badge]: https://badge.fury.io/py/googledevices.svg
[home]: https://ludeeus.github.io/ROOT
[platforms]: https://ludeeus.github.io/ROOT/platforms
[classes]: https://ludeeus.github.io/ROOT/classes
[methods]: https://ludeeus.github.io/ROOT/methods
[functions]: https://ludeeus.github.io/ROOT/functions
[cli]: https://ludeeus.github.io/ROOT/cli