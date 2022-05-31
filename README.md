# Hex Value Regex Tutorial
A regular expression, Regex for short, is an order of characters that describes a specific search pattern.

## Summary
This regular expression is matching a Hex Value. Description Below.
code snippet: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

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
### Anchors
This Hex Value expression has a ^ (carot or circumflex) and a $ (dollar symbol) anchors which means the expression will look for an exact string match. This means that the expression is looking for #?([a-f0-9]{6}|[a-f0-9]{3}) exactly.

### Quantifiers
This Hex Value expression has the ? (question mark) and two {} (curly brackets or curly braces) quantifiers in the expression. The ? means that the expresssion matches a string that has # followed by zero. The {6} and {3} means that the expresssion matches a string that has [a-f0-9] followed by 6 or 3 exactly.

### OR Operator
This Hex Value expression has a | (vertical slash or upright slash, meaning 'it is true that...' or 'such that...') and two [] (brackets, crotchets, closed brackets, or hard brackets) OR Operators. The ([a-f0-9]{6}|[a-f0-9]{3}) in this case means that the expresssion matches a string that has #? followed by [a-f0-9]{6} or [a-f0-9]{3} because of the |, but a-f0-9 in both statements are not captured because of the [].

### Character Classes
This Hex Value expression has not Chacter Classes (\d, \w, \s, meaning the expression matches a single character, word, or whitespace respectively).

### Flags
Although the Hex Value expression sits in between two / (forward slashes), the expression does not have any flags (g, m, or i after the last forward slash, meaning the expression is global, multi-line, or insensitive respectively).

### Grouping and Capturing
This Hex Value expression has () (parentheses). In the expression, [a-f0-9]{6}|[a-f0-9]{3} is grouped together inside the parentheses, but only the {6} or {3} are captured because the a-f0-9 statement sits inside the [], which means the satement will not be captured.

### Bracket Expressions
The [] is covered in the OR Operators section. In this case, the [a-f0-9] means that the expresssion matches a string that has any letter between a and f or any number between 0 and 9 or a mixture of the two.  

### Greedy and Lazy Match
The only greedy operators we have are our quantifiers (curly braces). They expand the match as far as they can.

### Boundaries
This Hex Value expression has no boundaries (\b before and after the expression. This means the expression will perform a whole words only search).

### Back-references
This Hex Value expression has no Back-references (\1, \2, etc, and \k, meaning the expression matches using the same text that was matched by the first, second, etc, capturing group).

### Look-ahead and Look-behind
This Hex Value expression has no Look-ahead or Look-behind statements (?= and ?<=, which means the content before the look-behind or the content after the look-ahead will not be part of the expression).

## Author
Jordan Stafford
(https://github.com/jowstafford)
