# REGEX TUTORIAL - Matching An Email

This tutorial provides a thorough yet concise explanation of the components that make up the regex for matching an email.

This regex is a sequence of characters that defines the specific search pattern used to identify a valid email address. It can be included in code or search algorithims in order to find certain patterns of characters within a string, or to find and replace characters or sequence of characters within the email string.

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

    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Anchors

    Anchors belong to the family of regex tokens that don't match any characters, but that assert something about the string or the matching process. Anchors assert that the engine's current position in the string matches a well-determined location: for instance, the beginning of the string, or the end of a line.

        "^"- this anchor is the beginning of an empty string
        "$"- this anchor signals an end to a string
        "\b"- this signals a word boundry
        "\B"- this signals not a word boundary

### Quantifiers

    ‹+› and ‹*›, when used outside character classes, are quantifiers. The plus sign repeats the preceding regex token one or more times, whereas the asterisk repeats it zero or more times. In these regular expressions, the quantified token is usually a character class, and sometimes a group. Therefore, ‹[A-Z0-9.-]+› matches one or more letters, digits, dots, and/or hyphens.

### OR Operator

    (.) is the match any operator
    `\*'operator repeats the smallest possible preceding regular expression as many times as necessary (including zero) to match the pattern.

### Character Classes

    ‹[A-Z0-9.-]› and other sequences between brackets are character classes. This expression allows letters between A and Z, digits between 0 and 9, and also literal dot and hyphen.

### Bracket Expressions

    ‹[A-Z0-9.-]› and other sequences between brackets are character classes. This expression allows letters between A and Z, digits between 0 and 9, and also literal dot and hyphen.

### Greedy and Lazy Match

    Greedy: i.e. '+)@('
    Lazy: ? , * , {}

    Regex engines are eager to return a match, which causes them to report the first  possible match found. This characteristic of regex's is referred to as "greediness".
        Any character followed by the + tells engine to repeeat the proceeding character as few times as possible.

## Author

This gist was created by Abigail Adams on @abigailGadams GitHub profile. Feel free to check out other content and share feedback! I hope you found this tutorial to be very informative.
