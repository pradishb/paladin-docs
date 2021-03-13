# place_offers

Places buy offers and sell offers. The offers are placed based on configuration from config.json.

### Configuration

| Field    | Data Type | Default | Description                                                                                                |
| -------- | --------- | ------- | ---------------------------------------------------------------------------------------------------------- |
| name     | string    | ""      | name of the item to place offer of                                                                         |
| stock    | string    | "0+"    | stock condition, accepts range, "0-100" or "100+"                                                          |
| price    | string    | "0+"    | accepted price range to make offer, also range                                                             |
| offer    | int       | 100     | bot's offer relative to best offer, if the best offer is 2000 and offer is 80, then bot places 80% of 2000 |
| count    | int       | 0       | how many items to place offer                                                                              |
| undercut | boolean   | false   | wheather to undercut an item or not, only supported for sell offers                                        |

**Example config.json**

```
{
  "place_buy_offers": [
    {
      "name": "rope belt",
      "stock": "0+",
      "price": "500-2000",
      "offer": 80,
      "count": 100
    }
  ],
  "place_sell_offers": [
    {
      "name": "rope belt",
      "stock": "0+",
      "price": "1000-3000",
      "count": 100,
      "undercut": true
    }
  ]
}
```

### Notes

- Market dialog must be open before using this action.
