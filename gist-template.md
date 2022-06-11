# Regex Tutorial By Brainybrian316

In this tutorial, I will be taking a brief look into Regex and how they work. My goal is to be able to write and use regular expressions in a way that is easy to understand and use.


## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components
***
### Anchors
Anchors are unique in that they match a position within a string, not a character.

Examples of Anchors are as follows: 

* `^` - Matches the beginning of the string. 

* `$` - Matches the end of the string. 
 
***
### Quantifiers

Quantifiers indicate that the preceding token must be matched a certain number of times. By default, quantifiers are greedy, and will match as many characters as possible.

Examples of Quantifiers are as follows: 

* `*` Star - Matches zero or more characters.
 

 * `+` Plus - Matches one or more characters.
 

* `?` Optional - Matches zero or one characters, effectively making it optional.

* `{n}` Quantifier - Matches exactly n characters.

***
### OR Operator

Known as Alternation... it acts like a boolean OR, matching one sequence or another.

Example of Alternation is as follows: 

* `|` Alternation - Acts like a boolean OR operator. Matches the expression before or after the `|` symbol.
 
***
### Character Classes

Character classes match a character from a specific set. There are a number of predefined character classes and you can also define your own sets.

Examples of Character Classes are as follows:

* `.` - Matches any character except linebreaks. 

* `\d` - Matches a  single digit.

* `\w` - Matches a single word character.

* `\s` - Matches a single whitespace character.

***
### Flags
Expression flags change how the expression is interpreted. Flags are used to modify the behavior of the expression.

Examples of Flags are as follows:

* `i` - Case Insensitive - Matches the expression ignoring case.

* `m` - Multi-line - Matches the expression across multiple lines.

* `s` - Dot All - Matches the expression across newlines.

***
### Grouping and Capturing

Groups allow you to combine a sequence of tokens to operate on them together.

Examples of Groups are as follows:

* `(abc)` - Groups multiple tokens together and creates a capture group for extracting.

 * `(?:)` - Groups multiple characters together without creating a capture group.

***
### Bracket Expressions
Bracket Expressions are characters enclosed by a bracket `[]` matching any single character within the brackets. 

Examples of Bracket Expressions are as follows:

* `[abc]` - Matches a character from the set.

* `[^abc]` - Matches a character that is not in the set.
 
* `[a-z]` - Matches a character from within the specified range of characters in the set.

***
### Greedy and Lazy Match

By default, quantifiers are greedy, and will match as many characters as possible. This is the behavior that is most commonly used in regular expressions.

However, you can make a quantifier lazy by adding a `?` to the end of the quantifier. This will make the quantifier match as few characters as possible.

Examples of Greedy and Lazy Match are as follows:

* `?` Lazy - Makes the preceding quantifier lazy, causing it to match as few characters as possible.

* `*?` Lazy Star 

 * `+?` Lazy Plus 

* `{n}?` Lazy Quantifier 

* `(abc)?` Lazy Group 

* `[abc]?` Lazy Character Class 

***
### Boundaries

Boundaries are used to match the start or end of a string. They are the places betwen characters kind of like a wall.

* `\b` - Matches a word boundary position between a word character and non-word character or position (start / end of string). 

* `\B` - Matches any position that is not a word boundary. This matches a position, not a character.

***
### Back-references

Back-references are used to match a previously matched group.

Examples of Back-references are as follows:

* `\1` - Captures the specified group in this case its the first group.

* `(?<name>abc)` - Creates a capturing group that can be referenced via the specified name.

***
### Look-ahead and Look-behind

Lookaround lets you match a group before (lookbehind) or after (lookahead) your main pattern without including it in the result. In addition, you can specify a positive or negative lookaround.
Negative lookarounds specify a group that can NOT match before or after the pattern.

Examples of Look-ahead and Look-behind are as follows:

* `(?=abc)` Positive Look-ahead - Matches the expression before the `?=` symbol.

* `(?!abc)` Negative Look-ahead - Matches the expression before the `?!` symbol.

* `(?<=abc)` Positive Look-behind - Matches the expression after the `?<=` symbol.

* `(?<!abc)` <mark>Negative Look-behind</mark> - Matches the expression after the `?<!` symbol.

***
## Author

My name is Brian Mojica, I am software engineer.  I have a passion for creating beautiful, functional, and intuitive user experiences. For more information about me, you can see my latest projects at my [GitHub](https://github.com/Brainybrian316) or view my [Portfolio](https://brainybrian316.com/).

If you wish to learn more about regex you can find more information provided on the  [Regex site](https://regexr.com/). 