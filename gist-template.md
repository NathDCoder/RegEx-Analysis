# An Analysis of Regex
Welcome to an overview of RegEx. Regex short for "regular expression" is niether a library or a programming language, but rather a sequence of characters used to create a pattern that can be used to validate, extract, substitute, or split strings.

## Summary
In the examples below we will focus on how to check if a string is Alphanumeric or not using RegEx. An alphanumerix RegEx will contain only alphabets from A-Z both lower and uppercase, as well as numbers 0-9. Our RegEx will check if the alphanumeric string we create meets all of the requirements.
Examples:

    The following string contains letters from the alphabet as well as numbers, so this ouput will be true.
    Input: string = JsOn123
    Output: true

    The following string only contains letters from the alphabet. Without umbers to complete it's requirements it will be false.
    Input: string = CsSForLife
    Ouput: false

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components
Regular Expressions also come with various components.
### Anchors
Anchors alow you to match a position before or after characters. 
 ^ – The caret anchor matches the beginning of the text.
 $ – The dollar anchor matches the end of the text.
### Quantifiers
The word quantifiers in JavaScript regular expression refers to the number of characters or expressions to match.
Here are a few examples:
n+ - used to match a string that contains one or more n
n* - used to match a string that contains zero, one, or more occurrences of n
n? - used to match a string containing zero or one occurrence of n
### Grouping Constructs
We can group constructs in Regex by placing the regex pattern inside parentheses.
For Example the regular expression (car) creates a single group containing the letters "c", "a", "r"
### Bracket Expressions
Bracket expressions indicate a set of characters to match.
Example:'Tiger'.match(/[abcdefg]/) // -> matches 'e' & 'g'.
### Character Classes
A character class is a special notation that matches any symbol from a certain set. 
Let's see how it works from the example below.
Example:
    let's say you have a phone# like this, but need to turn it into plain numbers.
    let phone = '+1-(718)-525-0107';
    let re = /\d/;
    console.log(phone.match(re));
    The console.log returns 14085550105 from using \d
### The OR Operator
The OR operator commonly seen as the pipe symbol "|" matches characters or expressions of either the left or right of the operator.
Example: String regex = "(t|T)";
This will match either lowercase or uppcase T.
### Flags
A flag is an optional parameter to a regex that modifies its behavior of searching.
Here are a list of them.
i - Makes the expression search case-insensitively.
g - Makes the expression search for all occurrences.
s - Makes the wild character . match newlines as well.
m - Makes the boundary characters ^ and $ match the beginning     
    and ending of every single line instead of the beginning and ending of the whole string.
y - Makes the expression start its searching from the index indicated in its   
    lastIndex property
u - Unicode	Makes the expression assume individual characters as code points, not 
    code units, and thus match 32-bit characters as well.
### Character Escapes
The backslash in a regular expression precedes a literal character. You also escape certain letters that represent common character classes, such as \w for a word character or \s for a space.
## Author
Hi there, I'm Nathanael Thomas a student of web developement and computer enthusiast. I hope you enjoyed reading about Regular Expressions and hope that this simplified it's use cases, so you can start using them in your future projects.  
