# Python Regular Expressions Tutorial

**Python Regular Expression**
Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not. They are used at the server side to validate the format of email addresses or passwords during registration, used for parsing text data files to find, replace, or delete certain string, etc. They help in manipulating textual data, which is often a prerequisite for data science projects involving text mining.

**Regular Expressions in Python**

>In Python, regular expressions are supported by the re module. The re library in Python provides several functions that make it a skill worth mastering.

**Basic Patterns:** Ordinary Characters

We can easily tackle many basic patterns in Python using ordinary characters. Ordinary characters are the simplest regular expressions. They match themselves exactly and do not have a special meaning in their regular expression syntax.

**Wild Card Characters:** Special Characters

Special characters are characters that do not match themselves as seen but have a special meaning when used in a regular expression. For simple understanding, they can be thought of as reserved metacharacters that denote something else and not what they look like.

Character(s) |	What it does
--------|--------
. |	A period. Matches any single character except the newline character.
^ |	A caret. Matches a pattern at the start of the string.
\A |	Uppercase A. Matches only at the start of the string.
$ |	Dollar sign. Matches the end of the string.
\Z |	Uppercase Z. Matches only at the end of the string.
[ ] |	Matches the set of characters you specify within it.
\ |	∙ If the character following the backslash is a recognized escape character, then the special meaning of the term is taken.
∙ | Else the backslash () is treated like any other character and passed through.
∙ | It can be used in front of all the metacharacters to remove their special meaning.
\w |	Lowercase w. Matches any single letter, digit, or underscore.
\W |	Uppercase W. Matches any character not part of \w (lowercase w).
\s |	Lowercase s. Matches a single whitespace character like: space, newline, tab, return.
\S |	Uppercase S. Matches any character not part of \s (lowercase s).
\d |	Lowercase d. Matches decimal digit 0-9.
\D |	Uppercase D. Matches any character that is not a decimal digit.
\t |	Lowercase t. Matches tab.
\n |	Lowercase n. Matches newline.
\r |	Lowercase r. Matches return.
\b |	Lowercase b. Matches only the beginning or end of the word.
`+` |	Checks if the preceding character appears one or more times.
`*` |	Checks if the preceding character appears zero or more times.
? |	∙ Checks if the preceding character appears exactly zero or one time.
∙ | Specifies a non-greedy version of +, *
{ } |	Checks for an explicit number of times.
( ) |	Creates a group when performing matches.
< > |	Creates a named group when performing matches.

 **Grouping in Regular Expressions**
The group feature of regular expression allows you to pick up parts of the matching text. Parts of a regular expression pattern bounded by parenthesis () are called groups. The parenthesis does not change what the expression matches, but rather forms groups within the matched sequence. You have been using the group() function all along in this tutorial's examples. The plain match.group() without any argument is still the whole matched text as usual