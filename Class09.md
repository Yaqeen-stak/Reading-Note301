# functional programming :

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

##  pure functions 

The first fundamental concept we learn when we want to understand functional programming is pure functions

* It returns the same result if given the same arguments (it is also referred as deterministic)

* It does not cause any observable side effects

It returns the same result if given the same arguments

## Reading Files

If our function reads external files, it’s not a pure function — the file’s contents can change.


## Immutability 

Unchanging over time or unable to be changed. 

When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value. 

### Referential transparency 

Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

`pure functions + immutable data = referential transparency`

### Functions as first-class entities 

The idea of functions as first-class entities is that functions are also treated as values and used as data.
Functions as first-class entities can:
* refer to it from constants and variables

* pass it as a parameter to other functions

* return it as result from other functions


# Map

The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values. 

# Reduce 

The idea of reduce is to receive a function and a collection, and return a value created by combining the items.




