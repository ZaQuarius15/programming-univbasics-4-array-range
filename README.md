# Array Range

## Learning Goals

- Demonstrate range
- Explain inclusive and exclusive range
- Generate an array with range

## Introduction

A range is a data set with start and end values, and a sequence of values in
between. Ranges can be found everywhere: The months January to December, the
numbers 0 to 9, lines 50 through 67 in code, and so on. Ruby supports ranges and
allows us to use ranges in a variety of ways. 

## Demonstrate Range

Ruby ranges are a set of values with a beginning and an end. The values in a
range can be numbers, characters, strings or objects. It is written using
`start_point..end_point` or `start_point...endpoint` literals. It provides
flexibility to the code and reduces its size.

Parenthesis are not necessary to define a range, but if you want to call methods
on your range you will need them.

The range class includes `Enumerable`, so you get all the powerful iteration
methods without having to convert the range into an array.


```ruby
for i in 0..3
    puts i
end

# => 0
# => 1
# => 2
# => 3
```
## Explain Inclusive and Exclusive Range

Ruby has two operators available to generate a range of values. The inclusive
two-dot `(..)` operator and the exclusive three-dot operator `(...)`. The
inclusive operator `(..)` includes both the first and last values in the range.
The exclusive `(...)` range operator excludes the last value from the sequence.
For example:

```ruby
1..10    # Creates a range from 1 to 10 inclusive
1...10   # Creates a range from 1 to 9
```

## Generate an Array With Range

The first and perhaps most natural use of ranges is to express a sequence.
Sequences have a start point, an end point, and a way to produce successive
values in the sequence. In order to convert a range to an array, we use the Ruby
`to_a` method. For example:

```ruby
(1..10).to_a -> [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```

## Conclusion

In this lesson we've discussed how ranges work in Ruby. With ranges, you can
better implement your own objects that support range and sequential operations.

## Resources

* [Ruby Ranges: How Do They Work?](https://www.rubyguides.com/2016/06/ruby-ranges-how-do-they-work/)
* [Ruby Ranges](https://www.techotopia.com/index.php/Ruby_Ranges)
* [Ranges in Ruby](http://rubylearning.com/satishtalim/ruby_ranges.html)
* [Ruby - Ranges](https://www.tutorialspoint.com/ruby/ruby_ranges.htm)
