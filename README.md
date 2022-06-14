# ruby-basics
basic ruby concepts that I have been learning.

* **nil** and **false** are the only two objects that evaluate to false in a boolean context.
* **to_s** return string value 
* to comment use **#** 
* i can access to character on string with [] 
* arrays access with nagative index and can access in parts. Exp: [-1], [0,5]
* to math operations can use **Math** class. Exp: Math.sqrt(4)
* no use ++ use +=

## Consol print
```
print -> print in same line
puts -> print and add \n
```
to print vars value in same text use #{*var_name*} into double quotes

## Arrays
* i cand append to end with push method or use << 

## Hashes
```
person_1 = { :name => "John", :age => 42 }
person_2 = { name: "Jane", age: 24 }        # alternate syntax
``` 
A colon followed by a name generates a Symbol object which corresponds one to one with the identifier

## methods
```
def name
  ...
end

def name(foo,bar)
  ...
end
```
## conditional
```
if a == 3
  puts "a is 3"
elsif a == 4
  puts "a is 4"
else
  puts "a is neither 3, nor 4"
end

puts "x is 3" if x == 3

puts "x is NOT 3" unless x == 3
```
* <=, <, >, >= - Comparison
* ==, != - Equality
* && - Logical AND
* || - Logical OR

### Case
```
case a
when 5
  puts "a is 5"
when 6
  puts "a is 6"
else
  puts "a is neither 5, nor 6"
end
```

## Loops
### each
```
data = [1, 2, 3]
data.each do |i|
  puts i
end
```
can also be used with key, value in |key, value|

### while
```
while conditional [do]
   code
end
```

### forin
```
for variable [, variable ...] in expression [do]
   code
end
```

## Exceptions
```
begin
    #... process, may raise an exception
rescue =>
    #... error handler
else
    #... executes when no error
ensure
    #... always executed
end
```
lauch exception with **raise**

## Class and objects
```
class Foo
  attr_accessor :instances,foo,bar  # provide class methods for reading/writing
  
  #constructor
  def initialize
    ...
  end
 ...
end

foo = nFoo.new
```
### inheritance
```
class Person
  ...
end

class Client < Person
  def initialize
    super
    ...
  end
 ...
end
```

## Modules
modules do not require an instance as classes do
```
module Foo
 ...
 def sum(a,b)
  ...
 end
end

include Foo
sum(a,b)
```
