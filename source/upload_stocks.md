# upload_stocks

Searches items in market and reads the item count. The collected data is uploaded to the manager.

## Configuration

### Fields

check_list: accepts a list of items to upload to the manager

config.json

```
{
  "upload_stocks": {
    "check_list": ["brown mushroom", "mana potion"]
  }
}
```

Market dialog must be open before using this action.
