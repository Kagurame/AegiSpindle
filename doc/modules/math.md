Spindle.Math
------------
Math module

* Shortname: Math
* Version: 1.0
* Author: Kagu-chan
* Source: [aegi-spindle-math.lua](https://github.com/Kagurame/AegiSpindle/tree/dev/src/aegi-spindle-math.lua)

> This module provides various math functions.

###Spindle.math.randomsteps(number min, number max, number step)
Returns a random value between min and max, but in given steps
```lua
local value = Spindle.math.randomsteps(1, 11, 2) -- Will result 1, 3, 5, 7, 9 or 11
```

###Spindle.math.trim(number x, number min, number max)
Trims a number value to be not lesser then min and not greater then max
```lua
local infade = Spindle.math.trim(30, 0, 300) -- Will return 30
local infade = Spindle.math.trim(-23, 0, 300) -- Will return 0
local infade = Spindle.math.trim(455, 0, 300) -- Will return 300
```

###Spindle.math.round(number x[, number dec])
Rounds a number to integer numbers or given decimal points if dec is given
```lua
local rounded = Spindle.math.round(33.33333) -- Will return 33
local rounded = Spindle.math.round(33.33333, 3) -- Will return 33.333
```

###Spindle.math.pythagoras(nil | bool | number a, nil | bool | number b[, number c])
Calculates all sides of a triangle - only one parameter can be false or nil, all number values have to greater than zero
```lua
Spindle.math.pythagoras(3, 3, nil) -- => 3, 3, 9
Spindle.math.pythagoras(3, 3) -- => 3, 3, 9
Spindle.math.pythagoras(3, nil, 9) -- => 3, 3, 9
Spindle.math.pythagoras(nil, 3, 9) -- => 3, 3, 9
```

###Spindle.math.between(number x, number min, number max)
Checks if x is between min and max or the same as one of them
```lua
Spindle.math.between(3, 2, 4) -- => true
Spindle.math.between(3, 4, 6) -- => false
```

###Spindle.math.buildWrapper()
Wrapper function for core application

