# Regex Tutorial: Matching an Email

Regular expressions (regex for short) are patterns of special characters that are used to match character combinations in strings.

## Summary

This is a regular expression for matching an email:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

It represents a search pattern meant for email validation. It checks to see if a string fulfills the following requirements for an email:

- The string must begin with an unspecified number of characters preceding the @ symbol. The characters can include lowercase letters, numbers between 0-9, an underscore, a period, and a hyphen.

- The string must include an unspecified number of characters between the "@" symbol and the "." symbol. The characters can include any Arabic numeral digits, lowercase letters, a period and a hyphen.

- The string must end with 2-6 characters following the "." symbol. The characters can contain lowercase letters and a period.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

Each component of the "matching an email" regex has a unique responsibility to make sure that a user enters a valid email address. We'll break down each component below.

NOTE: In our regex for matching an email example, the regex is created using literal notation which consists of a pattern enclosed between slashes. Javascript provides a second way to create a regex expression using a RegExp constructor. To learn more, review the MDN Web Docs on the RegExp object.

### Anchors

The ^ and $ characters are anchor components.

The ^ anchor matches the beginning of string. It checks that the string begins with the characters that follow it.

The $ anchor matches the end of the string. It checks that the string ends with the characters that precede it.

So in our “Matching an Email” regex, the string must start with something that matches the pattern `[a-z0-9_\.-]` and end with something that matches the pattern `[a-z\.]`.

Examples:

### Quantifiers

Quantifiers indicate the numbers of characters to match. They can set limits for a match such as the minimum and maximum number of characters that your regex is looking for.

`+` — Matches the pattern one or more times
`{}` — Curly brackets set limits for a match.
`{ n, x }` — Matches the pattern from a minimum of n number of times to a maximum of x number of times

### Character Classes

Character classes distinguish kinds of characters. They specify the characters that will successfully match a single character from a given input string. For example, character classes can be used to distinguish between letters and digits.

\d—Matches any Arabic numeral digit. This class is equivalent to the bracket expression [0-9].

### Grouping and Capturing

### Bracket Expressions

Anything inside a set of square brackets ([]) represents a range of characters that we want to match. They outline the characters we want to include.

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

### Escaping

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
