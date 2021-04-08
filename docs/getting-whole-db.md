# EASY DB - Getting whole Database

```js
db.all();
// AVAILABLE OPTIONS: { object: true }
// As an Argument to Receive just the Object

// EXAMPLE
db.set("owner", "BetaDv");
db.all();
// Result:
// [{ key: "owner", value: "BetaDv" }]

db.all({ object: true });
// Result:
// { owner: "BetaDv" }
```
