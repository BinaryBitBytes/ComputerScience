# Regex 101- Regular Expressions

## Introductory
---
A Regex is known as a Regular expressions, or regex for short, are a series of special characters that define a search pattern. We will navigate a search pattern bases on literal characters that will produce a regex search pattern with a result by deliminating meta characters withing each of the data sets to redact the required results to each of the respected regex components. In this document I will go about describing each of the respected regular expressions in detail and provide a functional example for each regular expression to better help the reader understand how the regular expressions are written and what they are doing.

## Summary
-------------

This document will introduce methods & solutions to provide the reader with the respected solutions that will supplement their understanding of regular expressions. Below in the table of contents I will address each of the topics in detail, provide supporting resources, and best explain and demonstrate these regular expressions with a functioning example. I will include a code snippet of each of the respected regex functions for the reader. In these running examples I will outline the meta characters and explain them such as; __\d for number__ and __. for any character__ as well as __* for 0 or more characters__ and also __combine .* for any character 0 or more__ of which is known as a __'wild card'__.

## Table of Contents
---------------
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components 
---------------

### Anchors

#### *__SOURCES__* :
---------------

>> - __https://www.regular-expressions.info/anchors.html__ : The caret ^ matches the position before the first character in the string and $ matches right after the last character in the string. __*Anchors do not match characters*__, *rather they match positions* of characters __*before, inbetween, or after*__ in a regular expression in a __specific position__ of a string or value. These searches on anchors can only find __zero-length matches__ but they can also be used to create searches for __*complications*__. A user can __trim the leading white space with the regex anchor function of: ^\s+__ and you can __match the trailing whitespace with the regex function of \s+$__. When dealing with a __string that runs multiple lines the regex command of \n indicates a *line break*__. Strings ending with multi line breaks can use regex functions in multi-line mode can leverage the __\Z__ to match before any number of trailing line breaks as well as the end of a string.

### Quantifiers

#### *__SOURCES__* :
---------------

>> - __https://docs.microsoft.com/en-us/dotnet/standard/base-types/quantifiers-in-regular-expressions__ : According to the Microsoft docs on *quantifiers* they are a specification of how many instances of a character, group, or character class that must be present in the input for a match to not be found. Examples of this can be expressed in __Greedy Quantifiers__ and __Lazy Quantifiers__. A few examples of a *greedy quantifier* inclue * (matched zero or more times), + (matches one or more times), ? (matches zero or one time), { n } (matches exactly n amount of times), { n ,} (matches atleast n times), and { n , m } (matches from n to m times). Lazy Quantifiers are referenced simalarly in the examples above the only difference is each of these examples above have a trailing ? mark at the end of the quantifier that make them a Lazy Quantifier.

>> - __https://www.regular-expressions.info/possessive.html__ : 

### Grouping Constructs

#### *__SOURCES__* :
---------------

>> - __https://docs.microsoft.com/en-us/dotnet/standard/base-types/grouping-constructs-in-regular-expressions__ : A __Grouping Construct__ portrays a subexpression of a regex and captures the substring of the input string. You can use these Grouping Constructs to:
1 Match a subexpression that is repeated in the input string.
2 Apply to a regex in a quantifier to a given subexpression that has multiple language elements.
3 Include grouping constructs in a subexpression in the string that is returned by the regex to us a regex.replace & match.result form of methods.
4 Retreive specific or individual subexpressions from the match.groups property and then process each one seperately from the entirety of a matches text.
These Grouping Constructs come in two types: __Capturing__ & __Noncapturing__.

__Grouping construct__	                        __*Capturing or noncapturing*__
- __Matched subexpressions__                    Capturing
- __Named matched subexpressions__	            Capturing
- __Balancing group definitions__	            Capturing
- __Noncapturing groups__	                    Noncapturing
- __Group options__	                            Noncapturing
- __Zero-width positive lookahead assertions__	Noncapturing
- __Zero-width negative lookahead assertions__	Noncapturing
- __Zero-width positive lookbehind assertions__	Noncapturing
- __Zero-width negative lookbehind assertions__	Noncapturing
- __Atomic groups__	                            Noncapturing

### Bracket Expressions

#### *__SOURCES__* :
---------------

>> - __https://www.ibm.com/docs/en/netcoolomnibus/8.1?topic=SSSHTQ_8.1.0/com.ibm.netcool_OMNIbus.doc_8.1.0/omnibus/wip/common/reference/omn_ref_re_bracketexpressions.html__ : According to IBM a *__Bracket Expression__* is used to match a single character or a collating element.The *hyphen* character (-) inbetween charecters within a bracket will __match ranges within the scope of those characters__. Using the __{ }__ *brackets* we can use the brackets with a combination of a number to declare a number of digits in a string to match. Using the carot symbol __^__ we can match any characters except those withing the square brackets, only if the carot is the first character after the opening [ or else it will be treated as a generic charecter and same applys to the hyphen (-). *Other Metacharacters withing square brackets will be treated as normal characters and do not require an escape character.*

__For Example:__
- __[b-g]__ : In this expression we will match characters b,c,d,e,f,g.
- __[xy7-9]__ : In this expression we will match x,y,7,8,9.
- __[yY] [eE] [sS]__ : In this expression we will match any spelling of yes, YES, Yes, YEs, yES and so on of any combination.
- __[^4-7]__ : Matches any characters and numbers except 4,5,6,7.
- __[.fu.]__ : Matches a multi-character collating element, such as fun.
- __[=t=]__ : Matches all collating elements with the same primary sort order as the element, including this element contained as itself.

>> - __https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap09.html__ : A __Bracket Expression__ is

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

I am BinaryBitBytes, a junior full stack developer learning the craft of coding like a a keyboard warrior. Here Is the link to the summary of Regex101 on my GitHub profile:
https://github.com/BinaryBitBytes/ComputerScience
