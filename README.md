# Array Range

## Learning Goals

- Demonstrate `Range`
- Explain inclusive and exclusive `Range`
- Generate an `Array` with `Range`

## Introduction

A `Range` is a subset of a collection between two markers. The markers we usually
use are the element indexes in an `Array`. When we provide a `Range` to an
`Array` it returns, a new, smaller `Array`.

Examples are:

* the months January to December
* the numbers 0 to 9
* lines 50 through 67 in code
* etc.

Ruby supports `Range`s and allows us to use `Range`s in a variety of ways. 

## Demonstrate Range

A `Range` is written using `start_point..end_point` or `start_point...endpoint`
literals. It provides flexibility to the code and reduces its size. The
difference between the two-dot (`..`) and three-dot (`...`) notation is whether
or not the last number of the `Range` should be included in it. With two-dot, it
is not; with three-dot, it is. This will be clear in the example below:

The `Range` is a powerful thing. You can invoke methods on it like this:
(1..3).size. If you want to invoke a method on a `Range` you have to wrap the
`Range` in `()` otherwise Ruby gets confused by all the dots. Here's the [range
documentation][range-doc] so you can see what `Range`s can tell you.

> **FUTURE GROWTH**: There's a beautiful and elegant reason for this that
> you'll be ready to understand when you get a bit more experienced in object
> orientation.


```ruby
for i in 0..3
  puts i
end
```

```text
0
1
2
3
```

```ruby
(0..3).size
#=> 4
```

## Explain Inclusive and Exclusive Range

Earlier we mentioned the "two-dot" and "three-dot" notation. Let's be a bit
more precise.

Ruby has two operators available to generate a `Range` of values. The inclusive
two-dot `(..)` operator and the exclusive three-dot operator `(...)`.

The inclusive operator `(..)` includes both the first and last values in the
`Range`.  The exclusive `(...)` `Range` operator excludes the last value from the
sequence.  For example:

```ruby
1..10    # Creates a range from 1 to 10, inclusive
1...10   # Creates a range from 1 to 9
```

## Generate an Array With Range

A natural and helpful use of `Range`s is to express a sequence.  Sequences have a
start point, an end point, and a way to produce successive values in the
sequence. In order to convert a `Range` to an `Array`, we use the Ruby `to_a`
method. For example:

```ruby
(1..10).to_a -> [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```

## Conclusion

In this lesson we've discussed how `Range`s work in Ruby. With `Range`s, you can
better implement your own objects that support `Range` and sequential operations.

## Resources

* [Range documentation][range-doc]
* [Ruby Ranges: How Do They Work?](https://www.rubyguides.com/2016/06/ruby-ranges-how-do-they-work/)
* [Ruby Ranges](https://www.techotopia.com/index.php/Ruby_Ranges)
* [Ranges in Ruby](http://rubylearning.com/satishtalim/ruby_ranges.html)
* [Ruby - Ranges](https://www.tutorialspoint.com/ruby/ruby_ranges.htm)

[range-doc]: https://ruby-doc.org/core-2.6.1/Range.html
