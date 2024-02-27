
# Validating Email Addresses with Regex

In modern web applications, validating user input is crucial to ensure data integrity and security. One common validation task is to verify the format of email addresses entered by users. In this project, we'll explore various regular expressions (regex) for validating email addresses and understand their components, strengths, and considerations. From simple validations to more robust patterns conforming to RFC standards, we'll delve into each regex variation step-by-step, providing insights into their design and usage.

## Summary

The regex we'll be discussing is a comprehensive pattern for validating email addresses, accommodating different levels of complexity and adherence to standards. Here's a summary of the regex pattern we'll explore:

```regex
^[A-Z0-9_!#$%&'*+/=?`{|}~^-]+(?:\.[A-Z0-9_!#$%&'*+/=?`{|}~^-]+)*@[A-Z0-9-]+(?:\.[A-Z0-9-]+)*$
```
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

Anchors in regular expressions define points in the string where the regex engine should start or stop matching. Commonly used anchors include:
- `^`: Matches the start of the string.
- `$`: Matches the end of the string.
- `\b`: Matches a word boundary.

### Quantifiers

Quantifiers control the number of times a character or group in a regex can appear. Common quantifiers include:
- `*`: Matches zero or more occurrences.
- `+`: Matches one or more occurrences.
- `?`: Matches zero or one occurrence.
- `{}`: Matches a specific number of occurrences, e.g., `{3}` matches exactly three occurrences.

### OR Operator

The OR operator, represented by `|`, allows for matching either one pattern or another. For example, `cat|dog` matches either "cat" or "dog".

### Character Classes

Character classes specify a set of characters that can match at a particular position in the string. They are defined inside square brackets, such as `[abc]`, which matches any of the characters 'a', 'b', or 'c'.

### Flags

Flags modify the behavior of a regex pattern. Common flags include:
- `i`: Case-insensitive matching.
- `g`: Global matching (matches all occurrences rather than stopping after the first match).
- `m`: Multi-line matching.

### Grouping and Capturing

Grouping is done with parentheses `( )` and is used to capture substrings within a match or apply quantifiers to multiple characters. Captured groups can be referenced later in the regex or in replacement patterns.

### Bracket Expressions

Bracket expressions, also known as character classes, allow you to specify sets or ranges of characters to match. For example, `[a-z]` matches any lowercase letter.

### Greedy and Lazy Match

Greedy matching matches as much of the string as possible, while lazy (or non-greedy) matching matches as little as possible. Greediness can be controlled with quantifiers like `*` and `+` by adding a `?` after them.

### Boundaries

Boundaries, such as `\b` for word boundaries, `\B` for non-word boundaries, `^` for the start of the string, and `$` for the end of the string, define the limits where matches can occur within the string.

### Back-references

Back-references allow you to reuse previously captured groups within a regex pattern. They are referenced using `\1`, `\2`, etc., where the number corresponds to the capture group.

### Look-ahead and Look-behind

Look-ahead and look-behind assertions allow you to match a pattern only if it is followed or preceded by another pattern, without including the matched text in the final match result. They are represented by `(?=...)` for positive look-ahead, `(?!...)` for negative look-ahead, `(?<=...)` for positive look-behind, and `(?<!...)` for negative look-behind.

## Author

git@github.com:Bdoherty1
