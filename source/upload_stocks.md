# upload_stocks

Searches items in market and reads the item count. The collected data is uploaded to the manager. This action is included in upload_my_offers action.

## Configuration

| Field      | Data Type       | Default | Description                                        |
| ---------- | --------------- | ------- | -------------------------------------------------- |
| check_list | list of strings | []      | : accepts a list of items to upload to the manager |

**Example config.json**

```
{
  "upload_stocks": {
    "check_list": ["brown mushroom", "mana potion"]
  }
}
```
