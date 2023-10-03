# Regex Tutorial: Matching an Email 

A regular expression, also known as as regex, is a sequence of characters that form a search pattern. Regular expressions allow developers to insure the integrity of user imput data, and are thus very valuable tools in data validation. In this vein, this tutorial provides an introductory understanding of the regular experssion used for matching and validating email addresses. 

## Summary

The regular expression featured in this tutorial is:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

As stated previously, this regular expression is used for matching and validating email addresses. It ensures that a user's input aligns with the standardized email format: a string of characters, an '@' symbol, another string of characters, a period, and the domain.

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

Anchors are characters used to define positions within searched or validated lines or strings. The two anchors in our regex are Caret '^' and Dollar '$'. Caret asserts that the match appears at the start of a line or string. Inversely, the Dollar asserts that the match appears at the end of a line or string.

### Quantifiers

Quantifiers specify the frequency of the preceding character, group, or character class to be matched. In this regex, Plus '+' is the quantifier, and it means that the preceding character or group will appear one or more times.

### OR Operator

Our regex does not contain an OR operator. In regular expressions, however, the OR operator is denoted by the pipe symbol '|', and it allows one to specify alternative patterns within a regex.

### Character Classes

A character class is a set of characters enclosed within square brackets '[]'. They allow for matching any one character within that set, and are used to define a character that will satisfy a part of a pattern. In this regex, the character class will match any lowercase letter, digit, underscore, period, or hyphen. Our regex uses several character classes, such as [a-z0-9_\.-]. 

### Flags

Our regex does not utilize flags. In regular expressions, however, flags are single-character modifiers that change the overall behavior of a regex. They tend to be added at the end of a regex pattern.

### Grouping and Capturing

Capturing groups, enclosed within parentheses (), treat multiple characters as a single unit and "capture" the matched text for later use. Our regex has three groups separating the local-part, domain, and domain suffix of the email address.

### Bracket Expressions

A bracket expression is a type of character class. It's used to specify a character class. In our regex, they are implemented to define the sets of characters in different parts of an email address.

### Greedy and Lazy Match

Our regex uses a greedy match, which means that the quantifier wants to match as many characters as possible in the input string. Inversely, in a lazy match, the quantifier matches as little content as possible. 

### Boundaries

Our regex does not include boundaries. In a regex, however, boundaries are assertions used to specify the position between characters, rather than the characters themselves. They dictate whether a character on the left side and a character on the right side are word characters and non-word characters. 

### Back-references

Our regex does not include back-references. Within the context of a regex, however, a back-reference refers to the reuse of previously-matched groups. Back-references allow for pattern-recognition and dynamic replacement operations.

### Look-ahead and Look-behind

Our regex does not include look-ahead or look-behind. Within the context of a regex, however, they are assertions that check whether a pattern following or preceding the main pattern exists. A look-ahead looks to what follows, while a look-behind looks at what precedes the current position.

## Author

I am studying at Columbia Engineering's Full Stack Bootcamp. For more information, please see my GitHub: https://github.com/tovalgreene.