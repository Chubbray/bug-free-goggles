# Title (My first tutorial)

Introductory paragraph (replace this with your text)

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
Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Anchors
^The        matches any string that starts with The -> 
end$        matches a string that ends with end
^The end$   exact string match (starts and ends with The end)
roar        matches any string that has the text roar in it

### Quantifiers
abc{2,5}    matches a string that has ab followed by 2 up to 5 c

### OR Operator

### Character Classes
\d         matches a single character that is a digit ->

.          matches any character ->

Use the . operator carefully since often class or negated character class (which we’ll cover next) are faster and more precise.

\d, \w and \s also present their negations with \D, \W and \S respectively.
For example, \D will perform the inverse match with respect to that obtained with \d.

In order to be taken literally, you must escape the characters ^.[$()|*+?{\with a backslash \ as they have special meaning.

### Flags
A regex usually comes within this form /abc/, where the search pattern is delimited by two slash characters /. At the end we can specify a flag with these values (we can also combine them each other):

m (multi-line) when enabled ^ and $ will match the start and end of a line, instead of the whole string

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
