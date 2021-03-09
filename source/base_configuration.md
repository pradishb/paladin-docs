# base_configuration

Base configuration that are not related to any actions.

### Configuration

| Field                   | Data Type | Default | Description                                                                                       |
| ----------------------- | --------- | ------- | ------------------------------------------------------------------------------------------------- |
| cast_spells             | boolean   | true    | wheather to cast spells in the background or not                                                  |
| sleep_if_last_character | int       | 1       | how long to sleep when the last character is logged out, useful for adding a delay for market-bot |

**Example config.json**

```
{
  "cast_spells": false,
  "sleep_if_last_character": 1800,
}
```
