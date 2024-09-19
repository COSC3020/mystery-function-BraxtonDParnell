# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

This function will return the middle element of an array. In the case that the array's length is an even number, it returns the higher middle element. Meaning, mystery([1,2,3,4]) will return 3.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```
