# EASY DB - Deleting Data

1. Standalone Data Removal:
```js
db.delete("Entry Name");

// EXAMPLE
db.set("user_1", { isDev:true, name:"BetaDv" });
db.delete("user_1");
// Removes the user_1 Entry.
```
2. Removing Data from Property:
```js
jd.delete("Entry Name");

// EXAMPLE
jd.set("user_1", { isDev: true, name: "BetaDv" });
jd.delete("user_1.name"); // Removes name from the user_1 Entry.
// Result:
// "user_1": { "isDev": true }
```
