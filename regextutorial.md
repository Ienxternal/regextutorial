# Title: Introduction to Regular Expressions (Regex)

As a web development student, I have developed a tutorial explaining a specifics of regex so that we can understand the search pattern the regex defines

## Summary:
A regular expression, or Regex, is a sequence of characters that defines a pattern used for string-searching algorithms, find and replace operations, and input validation. This guide provides an overview of Regex and its applications in various scenarios, along with explanations of key components and techniques.

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

    ### Anchors: Pinpointing Start and End
        ^abc$: An expression for exact string match.
            ^ asserts the start of the string or line.
            $ asserts the end of the string or line.
        \b\B: Detecting word and non-word boundaries.
            \b matches the position between word and non-word characters.
            \B matches positions not between word and non-word characters.

    ### Quantifiers: Controlling Repetition
        a*, a+, a?: Match characters zero or more, one or more, or zero or one times.
        a{5}, a{2,}, {2,6}: Define precise repetition counts.
        a+?, a{2,}?: Employing lazy quantifiers for minimal matching.
        ab|cd: Choosing between alternatives "ab" and "cd".

    ### OR Operator: Choices and Alternatives
        |: A versatile operator for alternatives.
        (cat|dog): Matches either "cat" or "dog".
        (apple|banana|orange): Selects among fruits.

    ### Character Classes: Selecting from Sets
        [ABC], [^ABC], [A-Z]: Defining character sets and ranges.
        .: A wildcard that matches any character except line breaks.
        \s\S, \w, \W, \d, \p: Predefined character classes.

    ### Flags: Expression Modifiers
        i, g, m, u, y, s: Altering the behavior of expressions.
        i: Case-insensitive matching.
        g: Global search to find all matches.
        m: Multiline mode for start and end anchors.
        u: Unicode mode for international character support.
        s: Dot (.) matches newline characters.

    ### Grouping and Capturing: Structuring Patterns
        (ABC), (?<name>ABC), \1, (?:ABC): Creating and referencing capture groups.
        (foo)(bar)\1\2: Matching "foobarfoobar".
        (?:foo)bar: Non-capturing group for precise grouping.

    ### Bracket Expressions: Custom Character Sets
        [aeiou]: Matches any vowel.
        [^aeiou]: Matches any non-vowel.
        [A-Z]: Selects uppercase letters.
        [0-9]: Matches digits.

    ### Greedy and Lazy Match: Balancing Efficiency
        Greedy: Matching the longest possible string.
        .*: Greedy matching.
        Lazy: Matching the shortest possible string.
        .*?: Lazy matching.

    ### Boundaries: Word and Line Delimiters
        \b, \B: Identifying word and non-word boundaries.
        \b\w+\b: Matches whole words.
        \B@: Matches "@" in email addresses.

    ### Back-references: Reusing Captured Text
        (<tag>).*?</\1>: Matches paired HTML tags.
        \b(\w+)\b\s+\1\b: Finds repeated words.

    ### Look-ahead and Look-behind: Advanced Constraints
        (?=ABC), (?!ABC), (?<=ABC>), (?<!ABC): Lookahead and lookbehind assertions.
        (?=\d+)\d{3}: Positive lookahead for a digit sequence.

    Conclusion: Harnessing Regex Mastery
        A summary of the covered concepts and techniques.


A short section about the author with a link to the author's GitHub profile https://github.com/Ienxternal
