# EASY DB - Easy Filtering

```js
db.startsWith("key", true / false);
// true / false is for Sorting (Optional)
// Searches for Any Entry in the Database that Starts with: "key"

// EXAMPLE
let i = 1
while(i < 8) {
  db.set("user_" + i, i);
  i++
}

let b = 1
while(b < 8) {
  db.set("ignore_user_" + b, b);
  b++
}
db.startsWith("user_");
// Result:
/* 
 [
   { entry: 'user_1', value: '1' },
   { entry: 'user_2', value: '2' },
   { entry: 'user_3', value: '3' },
   { entry: 'user_4', value: '4' },
   { entry: 'user_5', value: '5' },
   { entry: 'user_6', value: '6' },
   { entry: 'user_7', value: '7' }
 ]
*/
```
