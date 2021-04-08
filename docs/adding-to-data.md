# EASY DB - Adding to Data

```js
db.add("Entry Name", number);
// Number Must be an Integer

// EXAMPLE
db.set("betadv", { balance: 0, status: "poor" });
db.add("betadv.balance", 200);
// Adds to My Balance 200

db.set("betadv.status", "ok");
// Changes My Status
```
