# [JSON-DB](https://www.npmjs.com/package/@betadv/json-db)
A free Easy to Use JSON - DATABASE npm package.
In Beta currently, so Bugs may Occur!

## Features:
### - Automatic Database Creation
### - Data Adding / Setting
### - Data Removing
### - Data Retrieving
### - Sub-Property Support for Some of the Features Above

## How to Use:
### Creating Initial Database File:
```js
const jdb = require("@betadv/json-db");
jdb.createDB(/*Optional File Path Here, Default: "./database.json"*/);

// EXAMPLE
jdb.createDB("./important/database.json");
```

### Adding data to the Database:
1. Standalone Data:
```js
const jdb = require("@betadv/json-db");
jdb.set("Entry Name",/*Doesn't Support Standalone sub-property Edit for Now*/ "Entry Value");

// EXAMPLE
jdb.set("username_1", "BetaDv");
```

2. Entry with Sub-Data:
```js
const jdb = require("@betadv/json-db");
jdb.set("Entry Name",/*Doesn't Support Standalone sub-property Edit for Now*/ { Sub_Entry: "Sub Entry Value", "Sub_Entry_2": "Sub Entry 2 Value" });

// EXAMPLE
jdb.set("user_1", { name: "BetaDv", hobby: "Programming" });
```

### Removing Data:
1. Standalone Data Removal:
```js
const jdb = require("@betadv/json-db");
jdb.set("Entry Name",/*Supports Standalone Sub-Property Removal*/);

// EXAMPLE
jdb.set("user_1", { isDev:true, name:"BetaDv" });
jdb.del("user_1"); // Removes the user_1 Entry.
```
2. Removing Data from Property:
```js
const jdb = require("@betadv/json-db");
jdb.del("Entry Name",/*Supports Standalone Sub-Property Removal*/);

// EXAMPLE
jdb.set("user_1", { isDev:true, name:"BetaDv" });
jdb.del("user_1.name"); // Removes name from the user_1 Entry.
// So Result:
// "user_1":"isDev":true
```

### Retrieving Data:
1. Getting Standalone Data:
```js
const jdb = require("@betadv/json-db");
jdb.get("Entry Name");
/*Supports Getting Standalone Sub-Property Value*/

// EXAMPLE
jdb.set("username_1", "BetaDv");
jdb.get("username_1");
// Result:
// BetaDv
```
2. Getting Sub-Property Data:
```js
const jdb = require("@betadv/json-db");jdb.get("Entry Name");/*Supports Getting Standalone Sub-Property Value*/// EXAMPLE
jdb.set("user_1", { name: "BetaDv", isDev:true, luckyNumber:69, other: { isStupid:true } });
jdb.get("user_1.other.isStupid");
// Result:
// true
```

### [PACKAGE PAGE](https://www.npmjs.com/package/@betadv/json-db)
