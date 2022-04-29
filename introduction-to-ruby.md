# Introduction to Ruby

## Index

- [Introduciton to Ruby](#introduction-to-ruby)
    - [Overview & Sneak Peek](#overview-sneak-peek)
    - [Data Types: Numbers, Strings, Booleans](#data-types-numbers-strings-booleans)
    - [Math](#math)
    - [String Methods](#string-methods)
    - [Comments](#comments)
    - [Naming Conventions](#naming-conventions)
- [Putting the Form in Formatter](#putting-the-form-in-formatter)
    - [Getting Input](#getting-input)
    - [Printing the Output](#printing-the-output)
    - [Formatting with String Methods](#formatting-with-string-methods)

## Introduction to Ruby

### Overview & Sneak Peek

- High-level
- Interpreted
- Object-oriented
- Easy to use

### Data Types: Numbers, Strings, Booleans

```ruby
my_num = 25
my_boolean = true
my_string = "Ruby"

puts my_num
puts my_boolean
puts my_string
```

### Math

- Addition (`+`)
- Subtraction (`-`)
- Multiplication (`*`)
- Division (`/`)
- Exponentiation (`**`)
- Modulo (`%`)

### String Methods

```ruby
puts "Hello, World!".length # 13

puts "Hello, World!".reverse # "!dlroW ,olleH"

puts "hello, world!".upcase # "HELLO, WORLD!"
puts "HELLO, WORLD!".downcase # "hello, world!"
```

### Comments

```ruby
# I'm a single line comment

=begin
We are multi-line comments
We are multi-line comments
=end
```

### Naming Conventions

Start with a lowercase letter and words should be separated by underscores, like `counter` and `masterful_method`.
Ruby won't stop you from starting your local variables with other symbols, such as capital letters, `$`s, or `@`s, but by convertion these mean different things.

## Putting the Form in Formatter

### Getting Input

```ruby
print "What's your first name?"
first_name = gets.chomp
```

`gets` is the Ruby method that *gets* input from the user.
When getting input, Ruby automatically adds a blank line (or **newline**) after each bit of input;
`chomp` removes that extra line. (Your program will work fine without `chomp`, but you'll get extra blank lines everywhere.)

### Printing the Output

```
name = "g3un"
puts "Your name is #{name}!"
```

### Formatting with String Methods

```ruby
text1 = "abc"
text2 = text1.captialize # "Abc"
text1.capitalize! # "Abc"
```

We don't assign the result of `capitalize` to a variable.
Instead you might notice the `!` at the end of `captialize`.
This modifies the value contained within the variable `text1` itself.
