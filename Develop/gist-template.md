# Regular Expression Functions

A regular expression function is a function that is used to search for a specified string filtered by components within a large base of code or lettering. 

## Summary

This tutorial will hopefully help you to understand and start utilizing regex functions. We will talk about the different components, syntax, use-cases, and complexity of the regular expressions used in JavaScript.


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

    Ex: [^i*&2@] 

    the example above is a regular expression that contains any character other than an 'i', '*', '&', '2', or '@'.

    The syntax of a regex function contains these basic elements:
        -   '\' allows you to use a special character such as '$, ., *, ?, +, [], etc.
        -   '$' matches any pattern at the end of a string and nothing after it.
        -   '^' matches any pattern at the begining of a string and nothing before it.
        -   '[]' matches any character in the range set inside the brackets.
        -   '|' is used to indicate an OR operator.
        -   '()' is used to group multiple expressions.
        -   '+' is used to match 1 or more occurences.
        -   '?' is used to match 0 or 1 occurence of the element it follows.

### Anchors

    An Anchor used in a regular expression function are a certain type of token that doesnt match any characters. Instead, anchors ensure that the strings current position matches a well-determined position.

### Quantifiers

    Quantifiers used in a regular expression fucntion can be used to match a string one or more times but as little times as possible.

### OR Operator

    The OR operator within a regular expression is used to search for two specific strings.

    Ex: 
        fries | chips finds fries or chips

### Character Classes

    Wihin a regex function, character classes specify which characters will successfully match a single character from the given input string. Usually character classes are enclosed in brackets [].

### Flags

    Flags within a regex function are an optional parameter that modifies the behavior of searching. Usually implemented with special Anchors or Quantifiers.

    These consist of:
        i - ignores case-sensativity
        g - searches globally
        s - matches newlines
        m - used with '^' and '$' to search the beginning/ending of each line
        y - starts search at indicated property
        u - matches 32-bit characters
    

### Grouping and Capturing

    Grouping is used to group multiple patterns as one, wheras capturing provides extra submatch info.

### Bracket Expressions

    Bracket expressions are expressions enclosed in '[]'. These are used to specify a match between a certain set of single characters and can also contain multi-character elements.

### Greedy and Lazy Match

    A Greedy match uses an algorithm that for every position within the string it will try to match the pattern at that specific position and id there is no match it will search wihtin the next position.

    A Lazy match will use an algorithm almost opposite of a Greedy one. The lazy match will try to search the least minimal amount of times to try and find its match.

### Boundaries

    Boundaries are used in a regular expressions to differentiate a literal '^' in the search and actually using the '^' to specify the search at the beginning of the string. To set boundaries you would use '\' in front of the pattern.

    Ex: 
        '\^ fries' - will search for the literally '^' sign withing the string
        '^ fries' - will search at the begining of each line for 'fries'

### Back-references

    Back-referencing wihtin a regex is a way to search for the same text previously searched by a capturing group. 

### Look-ahead and Look-behind

    A Look-ahead assert (=) is used to tell the regex function what immediately follows the current position in the string. 
    A Look-behind assert (<=) is used to tell the regex function what is immediately precedes the current position in the string.

## Author

    Hello my name is Grant, I am a Full-Stack Developer who strives to continue learning forever.

    Github: https://github.com/mcnugboy

