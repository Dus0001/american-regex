# american-regex

Welcome to american-regex! Here you will find a desscriptive tutorial showing how to read Regular Expressions or "REGEX" for short. REGEX works by comparing a text against set parameters of a syntax created by the coder. This can be used in most software languages.

## Summary

For this turorial we will examine how to read syntax created for email address. The example is reflected by the following:  /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

The anchors define the start and end of an expression. "^" is the character used to indicate what the expression starts with. Conversely "$" represents what the expression ends with. Everything between these two anchors describe the syntax in entirety. 

### Quantifiers

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. * + ? and {} are the symbols that define the quantifier.  This is shown in our example following the period as ([a-z\.]{2,6})$/. The quantifiers are {2,6}, which maatches the string containing [a-z\.] for 2 or up to 6 copies. 

### OR Operator
The OR operator gives the ability to match a string against whats defined and include or exclude its target. Symbols that define an OR operator are for example a|b and a[b,c]. In our example the OR operator is not used.

### Character Classes
Character classes are defined by a character preceding a backslash. In our example we see it multiple times as '\da-z' and '\.- '. The first instance \da-z matched any digit a-z. The later \.- matches any character.

### Flags
Flags are used after character classes to add contingencies to the expression. The three flags are g (Global), m (multi-line) and i (insensitive). In our example there are no flags.

### Grouping and Capturing
Grouping is defined by parenthesis. This gives a clear distinction between ecaturing xpressions. In our example we have 3 instances of grouping. The first is the user handle, next is the server and last is the domain. 

### Bracket Expressions
These expressions are used define ranges for characters. This shortens the code eliminating inputing every possible character. This is seen in our code by [a-z\.]. The code within the braces shortens the occurence of any letter a-z. This has to be written within braces for the hyphen no to be literal.

### Greedy and Lazy Match
Greedy and Lazy match are versions of quantifiers that can expand your match broad or simple. Our code has instances of Greedy match in the example '[a-z0-9_\.-]+'. The plus sign instructs to look for the longest possible string of character. Lazy string would look for the shortest possible string defined by a question mark in repplacement of the plus sign.

## Author

This tutorial was created by Daven Steen who is an aspiring software developer currently enrolled in a coding bootcamp. 

Github Repository: https://github.com/Dus0001/american-regex
