# timezone

[![Build Status](https://drone.osshelp.ru/api/badges/ansible/timezone/status.svg)](https://drone.osshelp.ru/ansible/timezone)

The simple role which installs `tzdata` package and sets timezone.

## Usage (examples)

### The tzdata package installation only

```yaml
    - role: timezone
```

### The timezone setup only (without package installation)

```yaml
    - role: timezone
      timezone_setup: configure
      timezone_zone: Europe/Moscow
```

## Available parameters

| Param | Default | Description |
| -------- | -------- | -------- |
| `timezone_setup`| `full` | Setup mode. See [OSSHelp KB article](https://oss.help/kb4895) |
| `timezone_zone` | - | Timezone. See [list](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones) |

## TODO

...

## License

GPL3

## Author

OSSHelp Team, see <https://oss.help>
