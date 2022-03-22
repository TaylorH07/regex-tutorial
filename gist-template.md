# Title| Regex Tutorial

## Introductory paragraph

    - What is Regex? or in other words, what is Regular Expression? It is a sequence of characters that defines a specific search pattern. It is useful when extracting information from text, or to find certain patterns within a string. However, it is widely used to validate input.

## Summary

- Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
  - A Regex that matches all possible emails does not exist, but one that matches 99.9% of emails does. It a good practice to validate emails using regex, this will limit the user input upfront. For example, the growing mandatory usage of gmail.com and yahoo.com, which may run into scalability issues.

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

    - Anchors are not used to match a character, however they are used to match a position before, in-between, or after characters. The caret ^ is used for the character before the string, the $ is used to match with the last character of the string.
    - When there is a string with multiple lines, line are typically written first line\nsecond line (where \n indicates a line break). The ^ and $ and still be placed before and after the line-break (/n)

### Quantifiers

    - When encountered in a regular expression pattern, the regular expression engine interprets the *, +, ?, {, and } characters as quantifiers or part of quantifier constructs unless they are included in a character class.
        - The ? is a greedy quantifier matches the preceding element 0 or 1 time, which is equal to {0,1}
        - The {n} is a greedy quantifier that matches the n times, the lazy quantifier for this is {n}?. EX: the regular expression will look like  \ban?\b
        - The + is a greedy quantifier that matches a preceding element 1 or more times, which is equal to {1, }. EX: the regular expression will look like  \ban+\w*?\b
        - The * is a greedy quantifier that matches the preceding element zero or more times, it is equivalent to {0, }

### OR Operator

    - Grouping and alternation are core features of every modern regular expression library. When the or-operator is used, a user can provide as many terms as desired as long as they are separated with the | character.
        - EX: ^I like (cats|birds), but not (bears|giraffes).$ could match any of the the follow string:
                        I like cats, but not bears.
                        I like cats, but not giraffes.
                        I like birds, but not bears.
                        I like birds, but not giraffes.

### Character Classes

    - Also called character sets, can tell the regex engine to match only one out of several characters. To do so, you can place as many characters in between square brackets.
    EX: [A-Za-z_][A-Za-z_0-9]

### Flags

    - Flags are optional that allow functionality like global and case in-sensitive searching.
        - d generates indices for substring matches
        - g global search
        - i case in-sensitive search

### Grouping and Capturing

    -

### Bracket Expressions

    -

### Greedy and Lazy Match

    -

### Boundaries

    -

### Back-references

    -

### Look-ahead and Look-behind

    -

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
