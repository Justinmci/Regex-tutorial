# Regex-tutorial --Match an Email

## Summary

In this tutorial I will be explaining the use the regex (a sequence of characters that specifies a search pattern in text) using the expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ 

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

The anchors used for this regex expression are ^, this will indecate the begining of the string while the anchor $ is used to indicate the ending of the string.

### Quantifiers

One of the quantifiers used in the regex is {2,6}, this will allow a match range of 2-6 characters for a character set of [a-z\.]. Another quantifier is the + operator. + connects the users name, email service and .com. 

### Character Classes

The character class in this expression is \d, this this match single character digits from 0-9.

### Grouping and Capturing

Group one in the expression is ([a-z0-9_\.-]+) which matches the user email. Group two expression is ([\da-z\.-]+), this will match the email service. Group three is ([a-z\.]{2,6}), this captures the .com.

### Bracket Expressions

Email validation includes the bracked expression [a-z0-9_\.-], this is a case sensitive expression that'll aslo match letters a-z, numbers 0-9 and the characters -,.,_. The other bracked expression is [\da-z\.-], this will match case sensitive characters a-z, single digits from 0-9 and the characters .,-. [a-z\.] will match the character and the case sensitive characters a-z.

### Greedy and Lazy Match

The matching email regex includes two greedy matches. + will match as many times as possible while giving back as needed. The other being {} when matching `{2,6} for the last capture.

## Author

Here are some of my other projects at https://github.com/Justinmci 
