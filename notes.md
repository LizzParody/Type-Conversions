#Type Conversions

##Types in JavaScript

typeof undefined -> *undefined*
typeof array -> *object*
typeof null -> *object*
typeof NaN -> *number*
typeof Infinity -> *number*

###Difference betwwen *null* and  *undefined* 

*null* means no object
*undefined* means no value

### NaN
*NaN* Numeric values that are impossible to represent in JavaScript.
NaN is the only value in JavaScript that is not equal to itself!
```
NaN == NaN;
false
```

*Test for NaN*
```
isNaN(9);
false
```

```
isNaN(0/0);
true
