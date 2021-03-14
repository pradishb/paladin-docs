# check

Checks if a list of conditions satisfies or not. An action can be executed based on the result.

## Syntax

```
check <condtions>
```

**Example**

```
check hunt_conditions
```

## Configuration

| Field            | Data Type | Default | Description                                             |
| ---------------- | --------- | ------- | ------------------------------------------------------- |
| level_more_than  | int       | -       | checks if current level is more than the value          |
| level_less_than  | int       | -       | checks if current level is less than the value          |
| location         | list      | -       | checks if current location exactly matches the value    |
| is_near_location | list      | -       | checks if current location is closer to the value       |
| area             | string    | -       | checks if current minimap area is equal to the value    |
| on_success       | string    | -       | action to execute when all conditions are satisfied     |
| on_failure       | string    | -       | action to execute when all conditions are not satisfied |

**Example condtions "hunt" in config.json**

```
{
  "hunt_conditions": {
    "level_more_than": 8,
    "level_less_than": 9999,
    "on_success": "goto hunt complete",
    "on_failure": "goto hunt start"
  }
}
```

## Notes

- `on_sucess` and `on_failure` both can not be empty
