## Stand in Line - (Print using stringify) ❗

```js
function nextInLine(arr, item) {
    arr.push(item);
    return arr.shift();
    //remove 1 from the arrray and return it.
}

var arr = [1,2,3,4,5];

console.log("Before: " + JSON.stringify(arr));
//output Before: [1,2,3,4,5]
console.log("Before: " + arr);
//output Before: 1,2,3,4,5
console.log(nextInLine(arr, 6));
console.log("After: " + JSON.stringify(arr));
//output After: [2,3,4,5,6]
```

## Testing Objects for Properties - (hasOwnProperty) ❗

```js
var myObj = {
  gift: "pony",
  pet: "kitten",
  bed: "sleigh"
};

function checkObj(checkProp) {
  if (myObj.hasOwnProperty(checkProp)) {
    return myObj[checkProp];
  } else {
    return "Not Found";
  }
}

console.log(checkObj("gift")); // "pony"
console.log(checkObj("random")); // "Not Found"
```