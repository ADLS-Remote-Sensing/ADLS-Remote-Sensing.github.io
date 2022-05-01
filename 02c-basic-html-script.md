



```js
// create this function in the html file, 
// demonstrate it in the console. 
function years2days(years){
    console.log(years*365)
}; 
// Show how the result cannot be assigned to a variable
// in the console:

var myage_days;
myage_days = years2days(34);
myage_days;
```

Show how the function should `return` something rather than printing to the console.

```js
function years2days(years){
    return years*365
};
```



