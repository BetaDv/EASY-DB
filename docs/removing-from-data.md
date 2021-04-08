# EASY DB - Removing from Data:

```js
db.remove("Entry Name", number);
// Number Must be an Integer

// EXAMPLE
db.set("betadv", { balance: 200, status: "ok" });
db.remove("betadv.balance", 200);
// Subtracts from My Balance 200

db.set("betadv.status", "poor");
// Changes My Status
```
