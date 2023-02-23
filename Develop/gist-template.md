# Regex expressions


# Summary
A regular expression, commonly called regex, is a string of characters used to define a particular search pattern. It is utilized in coding or 
search algroithms to locate specific character patterns within a string or replace a sequence of characters in a string. Regular expressions 
are frequently employed to authenticate input as well.


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
- anchors are a type of regex components that start and ends a srting.
- to demonstrate how the anchor component would work in case of matching an email:
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$`
- The anchor ** ^ ** and ** $ ** show that the code must start with `/^([a-z0-9_\.-]+)`
and end with `.([a-z\.]{2,6})$`. to pass the matching test the given anchor component must begin and end with the prior parameters that were mentioned, so that no errors occur. 


### Quantifiers
- a quantifier component is used to decide how many times a particular character or group of characters reoccures or must be present to 
pass and match to the test.
- certain characters that are repeated often are as follows:
--`*` matches 0+ occurrences of the section that precedes it.
-- `+` matching more than one occurences of the sectio it follows.
-- `?` matches 0/1 occurences of the section it follows.
- for instance in the case of the match with an email:
-- the quantifier component will result in `([a-z0-9_\.-]+)`. This will ensure a match for any string that contains a-z, 0-9, _,.,or-.
The quantifier ** + ** states that the element must contain at least one of this criteria in order to qualify for a match.

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
