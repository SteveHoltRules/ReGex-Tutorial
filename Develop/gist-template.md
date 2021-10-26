# Regex

/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

Regular Expressions, known as regex, is a search tool that is used to comb through text to validate information. This can be a sentence to check for beginning a sentence with a capital letter and ending with punctuation, used for validating an email address, or used to validate a web address. This tool is available for use in many different programming languages.  

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
In Regex, there are different components that are used to signify checks against certain sections of the text, these components and their uses are shown below. 

### Anchors
Anchors signify a point to examine
^ Signifies the beginning of the string that is undergoing evaluation. In the above example the ^(https signifies the beginning that is required at the beginning followed by the set code of https.

### Quantifiers
{2, 6} This section is meant to match between 2 and 6 of the preceding token. If it was {2,} it would be 2 or more {6} would be exactly 6.
Another quantifier can be found at the end of the sample statement with the *, which specifies that the containing group should not contain the characters speficied in the group. 

### OR Operator
Alternation |
This gives varability to the match expression. The expression can match before or after the |.
m(u|e|a)d -> mud, med, mad. There are no or operators in the Regex example above.

### Character Classes
There are different cases of characters that are speficied in Regex. Every character is assigned to a category for reference. For instance a-z is contained in a different category than A-Z. Digits can be assigned through \d. All of these character classes are signified through a [] tag that contains the test to that is verified through Regex. These classes can also be escaped out of through the use of /, which can be used to specify a matching character. The character classes can also be further summarized through \w, \d\ , or \s which stand in place for word, digit, or whitespace. In the webaddress example, there is no stand-in for whitespace. 

### Flags
Flags can be used for different types of expressions. /aBc/i This is a flag that specifies that the whole expression is case sensitive. 

Another usefule flag is the global search will will retain the index of the last match and allow searches to return the same match.

When the multiline flag is enabled with beginning and end anchors ^ and \$ will match the start and end of the line, instead of the start and end of the whole string. Certain patterns with ^ and \$ with /m will include the multiline match. The flag at the end of the example is seen as $. 

When the unicode flag is enabled, you can use extended unicode escapes in the form.

There are no flags in the example Regex example shown above. 

### Grouping and Capturing
() Grouping is a method that is used to evaluate the string. The group string can run a match against the criteria in an order for compliance. 

### Bracket Expressions
[]The bracket highlights a character set. There are multiple character sets within this Regex file that are shown within the brackets. 

### Greedy and Lazy Match
b\w? Creates a match using a "b" - required, plus another (normal) charcater. () A Lazy match takes a preceding quantifier to match against as few characters as possible. By default quantifiers are greedy, meaning thaye will match as many characters as possible. 

### Boundaries
(\b) Sets the validation of the end of the word based on the value prior to the boundary. A boundary word position between a word character and a non-word character or position start and end of a string. (\B) Not word boundary, this will look the criteria that matches based on the position, so a @\B would mean that an s is required to be followed by another character. 

### Back-references
(?<name>ABC) creates a capturing group that can be referenced vai the specified name. This is used to match a pair of opening and closing tags that are passed in the string. In the beginning of the example statement, the :?/\ means that it is followed by. In the ? is also followed after the https. 

### Look-ahead and Look-behind
These are also called look-arounds. Look-ahead and look-behinds match characters with a pass/fail return instead of a match of a part of the character set. 

## Author

Matt Luna is a full stack web developer out of Dallas Texas who can be found tinkering in his workshop on the weekends or watching youtube to find a fix for just about anything. He can also be found on GitHub at https://github.com/SteveHoltRules
