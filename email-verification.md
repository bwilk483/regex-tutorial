# REGEX Tutorial

This tutorial to to help understand regular expressions or "Regex". Regex is a sequence of characters that specifies a search pattern in text.

## Summary

the Regex I will be describing is /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. this regex is used to verify emails and if the email follows the correct format.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors

Anchors are regex tokens that don't match any characters but that say or assert something about the string or the matching process. In the email verification regex /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ uses the ^ and $ anchor.

the ^ anchor

The caret anchor matches the beginning of the text like ^a would be true with a string of abc.
in the email verification regex the first part of the expression ^([a-z0-9_\.-]+). what this does is verifies that the beginning of a email contains only a threw z "a-z", 0 threw 9 "0-9", or these symbols "\_.-".

the $ anchor

The dollar anchor matches the end of the text like c$ would be true with a string of abc. in the email validation regex the last part of the expression is .([a-z\.]{2,6})$. what this does is verifies the end of your email like the .com or any other parts what it is saying is that it can be a threw z and must be at least 2 letter and cant be more then 4 letters.

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found.

In the email verification regex two quantifiers are being used one is + and the other is {n}.

the + quantifiers

what it + quantifiers is doing is connecting the parts of the email together /^([a-z0-9_\.-]+) @([\da-z\.-]+) \.([a-z\.]{2,6})$/. so lets break this down  into the parts. so thats use my email and break this down into the parts bwilk483@gmail.com or bwilk483 + @gmail + .com (the first part ^([a-z0-9_\.-]+) is for the bwilk483)+(the middle @([\da-z\.-]+) @gmail)+(the last part \.([a-z\.]{2,6})$ .com)

the {n} quantifiers

it the email verification regex the {n} quantifiers is at the end of the expression and is {2,6}. what this is saying it that the end can not be less then 2 letters or mor then 6

### Character Classes

In the context of regular expressions, a character class is a set of characters enclosed within square brackets. It specifies the characters that will successfully match a single character from a given input string. in the email verification regex it has a character class of \d

the \d character class

in the email verification regex the \d character class does is makes sure after the @ the the next letter is a-z \da-z

### Grouping and Capturing

Capturing groups are a way to treat multiple characters as a single unit. They are created by placing the characters to be grouped inside a set of parentheses. in the email verification regex it has 3 capturing groups.

the first is ([a-z0-9_\.-]+) in the email bwilk483@gmail.com this is for the bwilk483 part of the email

the second part is ([\da-z\.-]+) in the email above this is for the gmail part of the email.

the last part is ([a-z\.]{2,6}) and this is for the com of the email above

### Bracket Expressions

A bracket expression is either a matching list expression or a non-matching list expression. It consists of one or more expressions: ordinary characters, collating elements, collating symbols, equivalence classes, character classes, or range expressions.

in the email expression regex it uses [a-z0-9_\.-]. what this mean is the it contains letters from a-z that are case sensitive can have numbers 0-9 and also characters \_-. in the email.

## Author

this tutorial was made by Bryan Wilkerson

contact me at bwilk483@gmail.com

github https://github.com/bwilk483
