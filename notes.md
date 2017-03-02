# Type Conversions

## Types in JavaScript

typeof undefined -> **undefined** <br>
typeof array -> **object** <br>
typeof null -> **object** <br>
typeof NaN -> **number** <br>
typeof Infinity -> **number**

###Difference betwwen **null** and  **undefined** 

**null** means no object
**undefined** means no value

### NaN
**NaN** Numeric values that are impossible to represent in JavaScript.
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
Also
```
isNaN(0/0);
true
```

## Equality Operator (==)
Takes into account the types of the operands.
1. If the two values have the same type, just compare the values.
2. If the two values have different types, first it tries to convert them in the same types, and them compare them.

### Exceptions:

#### Comparing a *number* and a *string* 
```
5 == "5"
5 == 5
true
```
It converts the string into a number, and them compare them

#### Comparing *Boolean* and *any other type* 
```
true == 2;
1 == 2;
false
```
It converts the boolean into a number. True is converted to 1 and false to 0.

#### Comparing *null* and *undefined* 
```
null == undefined
true
```
It always evaluate to true. Both of those values means "no value" (a variable with no value and an object without value).

## Strict Equality (===)
Two values are strictly equal if the value and type is the same.
```
5 === "5";
false
```

## Addition and type conversion.
*number* and *string* 
```
5 + "5";
55
```
It converts the number into string and then concatenate the values.

Other arithmetic oparators (\*\), / , -) 
```
4 * "4" // 12
10 / "2" // 5
"7" - 2 //5
```
It converts the string into number.

## Convert string into number.
```
var num = 3 + Number("4"); // If it can't converted it will return NaN
```

## Equality of Objects
The object is equal to another object if the reference variable are pointing to the same object.
(When we test equality of two objects variables, we compare the reference of those objects).


# Truthy and Falsey
There are values in JavaScript that aren't true or false, but are treated as true or false.
Concentrate on what is falsey, everything else is truthy.
**Falsey**
* Undefined
* Null
* 0 
* NaN
* ""
