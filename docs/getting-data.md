# EASY DB - Getting Data

1. Getting Standalone Data:
```js
db.get("Entry Name");

// EXAMPLE
db.set("username_1", "BetaDv");
db.get("username_1");
// Result:
// BetaDv
```
2. Getting Sub-Property Data:
```js
db.get("Entry Name");

// EXAMPLE
db.set("user_1", { name: "BetaDv", info: { isStupid: true } });
db.get("user_1.info.isStupid");
// Result:
// true
```
