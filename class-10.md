# Error Handling & Debugging

![](https://image.slidesharecdn.com/error-handlinganddebugging-120524084901-phpapp02/95/error-handling-and-debugging-in-vb-2-728.jpg?cb=1337849468)

### JavaScript Errors - Throw and Try to Catch

##### The `try` statement lets you test a block of code for errors.

##### The `catch` statement lets you handle the error.

##### The `throw` statement lets you create custom errors.

##### The `finally` statement lets you execute code, after try and catch, regardless of the result.

#### Example:
```
    try {
    Block of code to try
    }
    catch(err) {
    Block of code to handle errors
    }
```

##### When an error occurs, JavaScript will normally stop and generate an error message.

##### The technical term for this is: JavaScript will throw an exception (throw an error).

### Range Error

##### A `RangeError` is thrown if you use a number that is outside the range of legal values.

##### For example: You cannot set the number of significant digits of a number to 500.

### Error Name Values

| Error Name | Description |
| ---------- | ----------- |
|EvalError | An error has occurred in the eval() function |
|RangeError | A number "out of range" has occurred |
|ReferenceError | An illegal reference has occurred |
|SyntaxError | A syntax error has occurred |
|TypeError | A type error has occurred |
|URIError | An error in encodeURI() has occurred |

### Eval Error

#### An `EvalError` indicates an error in the eval() function.

## JavaScript Debugging

#### Programming code might contain syntax errors, or logical errors.

#### Many of these errors are difficult to diagnose.

#### Often, when programming code contains errors, nothing will happen. There are no error messages, and you will get no indications where to search for errors.

#### Searching for (and fixing) errors in programming code is called code debugging.

