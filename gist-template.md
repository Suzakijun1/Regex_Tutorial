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

### Anchors

An anchor is a metacharacter that specifies a position within a string where a match should occur.
Within the Regex, the symbol `^` is the start of the string.

The symbol `$` is the position at the end of the string.

### Quantifiers

`?` matches the receding element zero or one time.
`*` matches the preceding element zero or more times.
`{2,6}` specifies a range for the preceding element (2 to 6 occurrences).

### OR Operator

`|` is used to specify alternatives.

### Character Classes

`[\da-z\.-]` matches any digit (`\d`), lowercase letter (`a-z`), dot (`.`), or hyphen (`-`).
`[a-z\.]` matches any lowercase letter (`a-z`) or dot (`.`).
`[\/\w \.-]` matches a forward slash (`\/`), any word character (`\w`), space (` `), dot (`.`), or hyphen (`-`).

### Flags

Flags are not used in the pattern.

### Grouping and Capturing

`(` and `)` are used for grouping and capturing subexpressions. In this example, there are four groups:
`(https?:\/\/)?` matches the protocol part of the URL (e.g., `http://` or `https://`). The `?` makes the preceding group optional.
`([\da-z\.-]+)` matches the domain name part of the URL. This group captures one or more digits, lowercase letters, dots, or hyphens.
`\.([a-z\.]{2,6})` match the top-level domain (TLD) part of the URL. This group captures a dot followed by 2 to 6 lowercase letters or dots.
`([\/\w \.-]*)*` matches the path part of the URL. This group captures zero or more occurrences of forward slash, word characters, spaces, dots, or hyphens. The `*` quantifier allows the group to repeat.
`\/?` matches an optional trailing forward slash.

### Bracket Expressions

bracket expressions, denoted by `[]`, define a set of characters to match.
`[\da-z\.-]` matches any digit, lowercase letter, dot, or hyphen.
`[a-z\.]` matches any lowercase letter or dot.
`[\/\w \.-]` matches a forward slash, word character, space, dot, or hyphen.

### Greedy and Lazy Match

By default, regular expressions are greedy, meaning they match as much as possible. For example, `.*` would match the longest possible sequence.
To make a quantifier lazy, you can add a `?` after it. For example, `.*?` would match the shortest possible sequence.

### Boundaries

Boundaries are used to match positions rather than specific characters. They include:
`\b` matches a word boundary (the position between a word character and a non-word character).
`\B` matches a non-word boundary.

### Back-references

Back-references allow you to refer to previously captured groups within the regex pattern.
They are denoted by `\` followed by a number (e.g., `\1`, `\2`, etc.) corresponding to the group index.
For example, `(abc)\1` matches "abcabc" since the first captured group is referenced.

### Look-ahead and Look-behind

Look-ahead and look-behind assertions are used to check if a pattern is followed or preceded by another pattern without including it in the match.
Look-ahead is denoted by `(?=...)`, where `...` represents the pattern to match ahead.
Negative look-ahead is denoted by `(?!...)` and asserts that the pattern does not match ahead.
Look-behind is denoted by `(?<=...)`, where `...` represents the pattern to match behind.
Negative look-behind is denoted by `(?<!...)` and asserts that the pattern does not match behind.

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

[GitHub Profile](https://github.com/Suzakijun1)

```

```
