# regex101

This is going to be a tutorial on the regular expression in particular for matching emails using the expression `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`. This expression can be used for numerous things such as text  editors, databases, etc..

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.
Regex or regular expression is a sequence of characters that can be used to define your search within your code using patterns. With the find and replace tool you are able to plug in this regex( `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` ), and single out all of the data that fit this criteria. This will find any information that has characters a-z,0-9
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

### Anchors
The Anchors in this particular expression are `^` and `$`. The `^` is is basically saying that this is going to be the start of the line or string, and `$` is saying that is going to be the end of the string or line. It is important to use these properly in order for the rest of your experssion to function properly.
### Quantifiers
The Quantifiers being used in this expression are `+` and `{2,6}`. The `+` operator is being used to connect the users email, with the service the user picked, and the `.com`. The `{2,6}` quantifer is what is allowing a match range of 2-6, for the character set of `[a-z\.]`.
### Grouping Constructs
The first group being constructed is `([a-z0-9_\.-]+)` this is saying that we want to match email names that include characters `a-z`, any digits from `0-9`,  `_`, `.`, and `-`. Next set of grouping is `([\da-z\.-]+)` which includes any digits`(\d)`, `a-z` again, underscores, periods, and hyhpens. Lastly, `([a-z\.]{2,6})`,  is saying that they want characters `a-z` and `.` for the .com.
### Bracket Expressions
Bracket Expressions is similar to what I was saying in [Grouping Constructs](#grouping-constructs). The first group is looking to match character `a-z` and any digits from `0-9`. Along with that, it will find  underscores, periods, and hyhpens. The second group is looking for any single digit(`\d`), `a-z` and also underscores, periods, and hyhpens. The third grouping is is simply getting characters `a-z` and a period.
### Character Classes
This regex doesnt have that many Character Classes, the first one is the range `a-z`. This is saying that it will gather characters from a to z. The next one is the `.` this can be used in a few different ways, if it is by itself it will match any character expect line breaks. Lastly is the `\d` which will match any single digit from 0-9.
### The OR Operator

### Flags

### Character Escapes

## Author
Nicholas Webb

Github: 
A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
