# Regex Tutorial

Regular expressions (regex) are the devices used as a search pattern and are made up of special characters.

## Summary

This template explains the pieces that are put together to match an username using a regular expression. /^[a-z0-9_-]{3,16}$/

The regex has to be wrapped within slashes (/).

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
Both ^ and $ are anchors.

The ^ as an anchor means the beginning of a string as the following characters.

    - As regex is case-sensitive, ^The would match the strings of "The" or "The animal", but not "the" or "the animal".

The $ anchor means the string ends with the characters before it. Just like the ^ character, it can be preceded by an exact string or just a range of potential matches. 

For the pattern [a-z0-9_-], our matching username string must start and end with a character within the pattern.

### Quantifiers

The section of the regex that is {3,16} means that the username must be between 3-16 characters long. This is a quantifier based off its curly brackets {}.

Curly brackets can create 3 different limits for a match as follows:

- { n } matches the pattern exactly n number of times
- { n, } matches the pattern at least n number of times
- { n, x } matches the pattern from a minimum of n number of times to a maximum of x number of times

So, for the {3,16} part of the regex, we want to find the preceding string pattern a minimum of 3 times and a maximum of 16 times. 

### OR Operator

The OR operator is the symbol (|). By using an OR operator, any combination of strings could be a match. 

For example: (cat):(dog) could be written with the OR operator making it (c|a|t):(d|o|g). This would allow the strings "cat:dog" and "cta:dgo" to be a match as well as "c:g", but "dog:cat" would not be.

### Character Classes

The Character Classes are the parts of the regex that describe what type of characters will potentially be included.

### Flags

Outside of the slash characters, at the end of the regex, a flag may be placed. Flags define additional functionality or limits of the regex. There are a total of 6 optional flags and they can be used concurrently or by themselves and have no ordering rules.

Common flags are: g - Global Search, i - Case insensitive search, and m - Multi-line search.

### Grouping and Capturing

Grouping and Capturing allows sections of the regex to be broken up to be checked for different constructs.

Typically you would group a section of the regex with parentheses (()) with each section within parentheses being subexpressions.

### Bracket Expressions

Bracket Expressions are anything set inside a set of square brackets ([]).

### Greedy and Lazy Match

Greedy would be the longest string match.

Lazy is the shortest string match.

### Boundaries

Boundaries can be found in the code by looking for the (\b). Essentially it tells the user that there is a word boundary in place.

### Back-references

Back-references are commands which refer to something that has already happened or was a match to part of the regex.

### Look-ahead and Look-behind

Look-ahead and Look-behind are also known as look around assertions and are similar to an anchor in that they search for a match. The difference is they can look around and match characters.

## Author

Hi, my name is Katie Marshall. I am just starting my journey as a software developer and I am really enjoying all that it entails. 

![Alt text](<images/Katie Marshall.png>)

https://github.com/katiesue378
