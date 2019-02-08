# Boolify

Boolify is a powerful boolean based module for Nodejs.

  - It is very fast, simple and robust. 
  - It is use for Validating whether argument is boolean
  - It is use for parsing to javascript Boolean value.

# Boolify Installation!
```
    npm  install --save node-boolify
```
# Boolify Setup!

- ES6 import
 ```
        import { isBoolean, Boolify } from "node-boolify";
```

- Javascript require
 ```
        var isBoolean = require('node-boolify').isBoolean;
        var Boolify = require('node-boolify').Boolify;
```

# Validation Results
```
        isBoolean(true); //true
        isBoolean('true'); //true
        isBoolean('TRUE'); //false
        isBoolean(1); //true
        isBoolean(2); //false
        isBoolean(false); //true
        isBoolean('false'); //true
        isBoolean('FALSE'); //false
        isBoolean(0); //true
        isBoolean(null); //false
        isBoolean(undefined); //false
        isBoolean(); //false
        isBoolean(''); //false

```
# Boolean Conversion Results
```
        Boolify(true); //true
        Boolify('true'); //true
        Boolify('TRUE'); //null
        Boolify(1); //true
        Boolify(2); //null
        Boolify(false); //false
        Boolify('false'); //false
        Boolify('FALSE'); //null
        Boolify(0); //false
        Boolify(null); //null
        Boolify(undefined); //null
        Boolify(); //null
        Boolify(''); //null
```