# Title (replace with your title)

Regex, short for Regular Expression, is a sequence of characters that forms a search pattern. It is primarily used for pattern matching and manipulating text strings. In a regular expression, characters can represent themselves or serve as metacharacters with special meanings. By combining these characters and metacharacters, you can create complex patterns to match specific strings or patterns within a larger text. Some common uses for regular expressions include: Pattern matching, string manipulation, text parsing, etc.

The following gist will give a thorough description of the central components in matching a given URL utilizing regular expressions in Javascript.

## Summary

The following regex can be used in order to validate a URL.

```
Regex Matching a URL:
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
```

The following gist will break down this regex by its components (anchor, quantifies, grouping constructs, bracket expressions, character classes, and character escapes). Each section will have a description, symbol, and where the code is located within the regex.

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

An anchor is a metacharacter that specifies a position within a string where a match should occur.
Within the Regex, the symbol `^` is the start of the string.
Here is the full regex:

```
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]_)_\/?$/

```

### Anchors

### Quantifiers

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

[GitHub Profile](https://github.com/Suzakijun1)

```

```
