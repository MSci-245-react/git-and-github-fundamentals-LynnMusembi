# Week 1 Takeaways & Key Learnings - MSE 245
In lecture 1, I learned that `let` is block scoped but `var` escapes functions
- `let`: block-scoped
- `var`: function-scoped
### *Using var to declare a variable*
```javascript
// Using var to set y
function sum() {
  var x = 5
  if (x>0) {
    var y = 3
  }
  console.log(y)}
sum ()
```
```javascript
// Output
undefined 
3
```
### *Using let to declare a variable*
```javascript
// Using let to set y
function sum () {
  var x = 5
  if (x>0) {
    let y = 3 
  }
  console.log(y)}
sum ()
```
```javascript
// Output
undefined
Uncaught ReferenceError: y is not defined
    at sum (REPL52:6:13)
```
