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
- The OR operator also denote as | operator ( `|` refers to the logical OR)
- It can be used to match characters or expressions of either the left of the right side of the ** or operator**
- In the instance of match an email `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})`- the OR operater is not present.
- A possible example of an OR operater could be found in the matching HTML Tag - `/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/` - whrein  the left side `/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>` is seperated with the `|` from the right side `\s+\/>)$/`.
### Character Classes
- a character class refers to a set characters  enclosed within a square bracket`[]`.
- character classes specify the characters that will be successfully match a single character from a probided input string.
SYNTAX
-** d ** - matches a single character that is a *digit* between 9 and 0.
-** w ** - matches a *word* character [A-Za-z0-9_]
-** s ** - matches *whitespace* character 
-** D ** - matches a *NON-digit* character
- In the case of matching the email properly: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})`
-- `\d` represents a single digit ranging from the numerical values 9 to 0 after the `@` sign in the email.
This string will only match a single digit such as "2", but not "22" or "12".

### Flags

### Grouping and Capturing
- capturing groups is a method used to group or to enclose multiple characters in one unit.
- These groups are created by placing the characters to be grouped inside a set of parenthesis.
- in the instance of matching an email address : `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})`
-- `([a-z0-9_\.-]+)`- first grouped characters in our regex code would match the email name.
--`([\da-z\.-]+)`- the second grouped characters in our regex code would mstch the email service for example yahoo. 
-- `([a-z\.]{2,6})`- the third grouped characters in our regex code would match the domain such as .com.

### Bracket Expressions
A bracket expression, enclosed in square brackets [], is a component of regular expressions that is used to match a specific set of single characters or a specific set of multi-character collating elements, based on the list expressions contained within the bracket expression.

When matching an email address using the regular expression`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`, the bracket expressions are used to match certain characters. The expression [a-z0-9_\.-] matches any lowercase letter from a to z, numerical characters from 0 to 9, as well as characters such as _, -, and ..

Similarly, the expression [\da-z\.-] matches any numerical character from 0 to 9, any lowercase letter from a to z, as well as the characters . and -. The expression [a-z\.] matches any case-sensitive character from a to z, as well as the character .


### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
