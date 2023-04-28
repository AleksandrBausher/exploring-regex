# Exploring Regex: A Beginner's Guide to Regular Expressions

Regex is a helpful tool for working with text data. It can search for specific patterns of text and modify them in useful ways. This is useful for people who work with text a lot, like programmers and data analysts. Regex is used in many different programs, like text editors and command-line tools. By learning Regex, you can get better at working with text data, which is important for many jobs.

## Summary

A regex for matching a URL

```
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
```

This regex is used to find URLs in a string. It looks for patterns that start with "http://" or "https://", followed by a domain name and top-level domain, and optionally followed by a path or query string.

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

Regex is made up of different parts that define a search pattern. These parts include literal characters that match themselves, special characters called metacharacters that have specific meanings, sets of characters called character classes that match any character in the set, quantifiers that specify how many times a character or group should occur, and grouping constructs that group characters or expressions together. By using these parts together, we can create complex patterns that can find and change text in a very flexible and efficient way.

### Anchors

Anchors are special characters in Regex that define the position of a pattern in a string. There are two types:

In the regex, the ^ and $ symbols are anchors. The ^ symbol matches the start of the string and the $ symbol matches the end of the string. Together, they ensure that the regex matches the entire string and not just a part of it.

### Quantifiers

In Regex, quantifiers are special characters that determine the number of times a character or group should occur. They specify how many times a character or group should be matched, and can help to make a search pattern more precise. There are several quantifiers in Regex, including:

The asterisk \*: This quantifier matches zero or more occurrences of the preceding character or group.

The plus sign +: This quantifier matches one or more occurrences of the preceding character or group.

The question mark ?: This quantifier matches zero or one occurrences of the preceding character or group.

Curly braces {}: These quantifiers allow you to specify an exact number of occurrences. For example, {3} matches exactly three occurrences, and {2,5} matches between two and five occurrences.

Quantifiers can be very useful for creating more complex search patterns that match text in a specific way.

### OR Operator

In Regex, the or operator | is a metacharacter that represents a logical OR between two expressions. It allows you to match one pattern or another in a given string.

For example, if you want to find either the word "cat" or "dog" in a string, you can use the regular expression cat|dog. This will match either "cat" or "dog" in the string, regardless of the order or context in which they appear.

The or operator can be useful for creating more complex search patterns that involve multiple alternatives. It is also commonly used in combination with grouping constructs to create more complex expressions.

### Character Classes

In Regex, character classes are sets of characters enclosed in square brackets [] that match any character in the set. They provide a way to match any character from a specific group or range of characters.

For example, the regular expression [aeiou] matches any lowercase vowel in a string. Similarly, the regular expression [0-9] matches any digit from 0 to 9.

Character classes can also be negated by placing a caret ^ inside the square brackets. For example, the regular expression [^aeiou] matches any character that is not a lowercase vowel.

Character classes can be very useful for creating more precise search patterns that match specific types of characters in a given string.

### Flags

In Regex, flags are additional parameters that can be added to a regular expression to modify its behavior. They are represented by one or more characters at the end of the regular expression, after the closing slash /.

There are several flags in Regex, including:

i: This flag makes the regular expression case-insensitive, meaning it will match both uppercase and lowercase characters.

g: This flag makes the regular expression global, meaning it will match all occurrences of the pattern in the input string, rather than just the first occurrence.

m: This flag makes the regular expression multiline, meaning it will match patterns across multiple lines, rather than just a single line.

Flags can be very useful for modifying the behavior of a regular expression to better suit a particular use case. They can also be combined to create more complex regular expressions with more precise matching behavior.

### Grouping and Capturing

In Regex, grouping and capturing are used to combine and extract parts of a match. Parentheses are used to group the expressions together and you can apply metacharacters or quantifiers to them. This enables you to capture and isolate specific parts of a match, which can be used later in the regular expression or in your code. It's useful for extracting and using specific information from a matched string.

### Bracket Expressions

In Regex, square brackets [] are used to match a single character from a set of characters. For instance, [aeiou] matches any vowel character, while [a-z] matches any lowercase letter. The caret ^ at the beginning of a bracket expression negates it. Therefore, [^aeiou] matches any character that is not a vowel. Bracket expressions are useful for matching specific character sets in a string and can be combined with other Regex components to create more complex matching patterns.

The bracket expression in the given regex is [\da-z.-]+, which matches one or more characters that are either digits (\d), lowercase letters (a-z), dots (.), or hyphens (-).

### Greedy and Lazy Match

In Regex, greedy and lazy matching are two ways to match patterns in text. Greedy matching tries to match as much text as possible that meets the pattern, while lazy matching tries to match as little text as possible. The difference is shown in the use of + and \* quantifiers. The choice of quantifier affects the outcome of the match, and it is important to select the right one when working with complex patterns and large amounts of data.

### Boundaries

In regex, boundaries are used to specify the position of a match within a string. There are two types of boundaries: ^ (caret) matches the position at the start of a string and $ (dollar) matches the position at the end of a string. Additionally, \b matches the position between a word character and a non-word character, while \B matches the position between two word characters or two non-word characters. Boundaries are useful for creating more complex patterns for text matching and manipulation by combining them with other regex components like character classes, quantifiers, and capturing groups.

### Back-references

In regex, back-references allow you to refer to a previously matched group within the same pattern. This is done by putting the group number in parentheses with a backslash, like \1. This lets you match the same text as the original group.

Back-references are a useful tool for matching and manipulating text in complex ways. They are often used in find-and-replace operations to modify specific parts of a string.

### Look-ahead and Look-behind

Assertions in regular expressions, commonly known as look-ahead and look-behind, are used to match a pattern only if it is followed or preceded by another pattern. Look-ahead assertions are used to match the pattern only if it is followed by the specified pattern, and are denoted by (?=pattern). Conversely, look-behind assertions are used to match the pattern only if it is preceded by the specified pattern, and are denoted by (?<=pattern). Negative look-ahead and look-behind assertions can also be used to indicate that the pattern should not be followed or preceded by another pattern, and are written as (?!pattern) and (?<!pattern) respectively. Although these assertions can create more complex regex patterns for text manipulation, they can be more computationally expensive and should be used wisely.

## Author
Learning enthusiast who is willing to make his full stack coding skills growing by practicing and learning new tech details on daily basis.
[AleksandrBausher](https://github.com/aleksandrbausher)
