# hunt

Hunt configuration is using when using hunt actions (hunt_node, hunt_stand).

### Configuration

| Field       | Data Type | Default     | Description                                                                                     |
| ----------- | --------- | ----------- | ----------------------------------------------------------------------------------------------- |
| kite        | boolean   | true        | wherher to kite (keep distance) from enemies, use false for knight and true for other vocations |
| chase       | boolean   | false       | if true, bot turns on chase mode, useful for knights, use false for other vocations             |
| comabt_mode | string    | "offensive" | which combat mode to use when hunting, options: "offensive", "defensive", "balanced"            |

**Example config.json for knights**

```
{
  "hunt": {
    "kite": false,
    "chase": true,
    "combat_mode": "offensive"
  }
}
```
