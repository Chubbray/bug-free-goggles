# Title (How to wright an e-mail code)

Introductory paragraph (replace this with your text)

I am Kenneth Sorensen, this is my first tutorial and I chose to do it on matching an e-mail. I have often wondered how when you put in an e-mail address onto a form, how it knows if it is a valid e-mail. So lets get stated and if there is anything I missed or you would like to add please do so in the comments. 

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

 I will try and attempt to explain to you how to wright the code to make this happen. The code example is: Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. I will try and break down each section to make it easier to understand.

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
/^/([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})/$/

^The        matches any string that starts with The -> 
end$        matches a string that ends with end
^The end$   exact string match (starts and ends with The end)
roar        matches any string that has the text roar in it

### Quantifiers
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]/{2,6}/)$/

abc{2,5}    matches a string that has ab followed by 2 up to 5 c

### OR Operator

### Character Classes
/^([a-z0-9_\.-]+)@([/\da-z\.-/]+)\.([a-z\.]{2,6})$/

\d         matches a single character that is a digit ->

.          matches any character ->

Use the . operator carefully since often class or negated character class (which we’ll cover next) are faster and more precise.

\d, \w and \s also present their negations with \D, \W and \S respectively.
For example, \D will perform the inverse match with respect to that obtained with \d.

In order to be taken literally, you must escape the characters ^.[$()|*+?{\with a backslash \ as they have special meaning.

### Flags
( / ) ^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$ ( / )

A regex usually comes within this form /abc/, where the search pattern is delimited by two slash characters /. At the end we can specify a flag with these values (we can also combine them each other):

m (multi-line) when enabled ^ and $ will match the start and end of a line, instead of the whole string

### Grouping and Capturing

### Bracket Expressions
/^(/[a-z0-9_\.-]/+)@([\da-z\.-]+)\.(/[a-z\.]/{2,6})$/

[abc]            matches a string that has either an a or a b or a c -> is the same as a|b|c -> Try it!
[a-c]            same as previous

Remember that inside bracket expressions all special characters (including the backslash \) lose their special powers: thus we will not apply the “escape rule”.

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
