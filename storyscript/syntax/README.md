---
prev: /storyscript/intro/
next: /storyscript/execution/
---

# Syntax

The following is a brief overview of Storyscript's main features. Head to the next chapter for an in-depth explanation of the individual features.

```coffeescript
###
Meet Storyscript
###

# Pull data from a microservice
output = service action key:value
output = team/service action key:value
# Discover and create services in the Storyscript Hub

# Call a function
output = function_name(key:value)
# A Storyscript function
# or another programming language

# Call type methods
output = variable mutation key:value

# Event streaming microservice
when service action event key:value as output
    ... # run this block for every event

# Types
string = "Hello"
integer = 1
number = 1.3
bool = true
list = ['a', 'b', 'c']
map = {'apple': 'red', 'banana': 'yellow'}
regexp = /^foobar/
empty = null
time = 1d35m

# Destructuring
{ apple, banana } = map
# apple = 'red'

# Conditions
if one > 1
    # ...
else if one == 1
    # ...
else
    # ...

# Loops
foreach list as item
    # ...
while true
    # ...

# Functions
function name input:int returns int
    # ...
    return input
name(input:1)
# >>> 1
```
