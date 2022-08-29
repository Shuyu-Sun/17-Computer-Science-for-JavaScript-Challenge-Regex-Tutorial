# 17-Computer-Science-for-JavaScript-Challenge-Regex-Tutorial

A regular expression is a sequence of characters that forms a search pattern. The user can define waht needs to be searched in a text with the help of regular expressions.</br>
Regular expressions can be of any number of characters, be it alphabet, digits or special characters.

## Summary

Regular expressions are more commonly used for text search and text replacement operations.</br>
General Syntax:</br>
/pattern/flag

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

### Quantifiers
Quantifiers define the number of occurrences of a string. Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. </br>
```+``` Indicates one or more occurence of the character.</br>
```*``` Indicates zero or more occurences of the character.</br>
```?``` Indicates zero or one occurence of the character.</br>

### OR Operator
/([a-z1-3]{6}|[a-f7-9]{8})/
The "or" operator within a regular expression is defined using the ```|``` element. The or operator indicates that it could either of the components that we are separating with the ```|```. For our hex value regular expression we have ([a-z1-3]{6}```|```[a-f7-9]{8}). Note the or operator separating these 2 components. 

### Character Classes
Character classes are components within our regular expression that tells us what type of characters to expect. In our example our character classes are confined within brackets ```[]```.

### Flags
There are several flags you can specify to alter the behavior of a regular expression. Flags may be appended to the end of a regex literal or they may be specified as the second argument to the Regular expression.</br>
- ```g``` Global. </br>
Finds all matches instead of stopping after the first.</br>
- ```i``` Ignore case.</br>
/[a-z]/i is equivalent to /[a-zA-Z]/</br>
- ```m``` Multiline.</br>
^ and $ match the beginning and end of each line respectively treating \n and \r as delimiters.</br>
- ```u``` Unicode.</br>
If this flag is not supported you must match specific Unicode characters with \uXXXX where XXXX is the character's value in hexadecimal.</br>
- ```y``` Finds all consecutive/adjacent matches. </br>

### Grouping and Capturing
Capturing groups are a way to treat multiple characters as a single unit. They are created by placing the characters to be grouped inside a set of parentheses. For example, the regular expression (dog) creates a single group containing the letters "d" "o" and "g" .

### Bracket Expressions
```[abcd]```</br>
Matches any character in the square brackets.</br>
```[a-d]```</br>
Matches any character in the range of characters separated by a hyphen ( - ).</br>
```[^abcd] [^a-d]```</br>
Matches any character except those in the square brackets or in the range of characters separated by a hyphen ( - ).</br>
```[.ab.]```</br>
Matches a multi-character collating element.</br>
```[=a=]```</br>
Matches all collating elements with the same primary sort order as that element, including the element itself.</br>

### Greedy and Lazy Match
'Greedy' means match longest possible string.</br>

'Lazy' means match shortest possible string.</br>

For example, the greedy ```h.+l``` matches 'hell' in 'hello' but the lazy ```h.+?l``` matches 'hel'.

### Boundaries
- Before the first character in a string if the first character is a word character.</br>
- After the last character in a string if the last character is a word character.</br>
- Between two characters in a string if one is a word character and the other is not.</br>

### Back-references
back-references are regular expression commands which refer to a previous part of the matched regular expression. Back-references are specified with backslash and a single digit (e.g. ' \1 '). The part of the regular expression they refer to is called a subexpression, and is designated with parentheses.

### Look-ahead and Look-behind
Highly recommand using an oline editor http://regexr.com to test out your Regular Expressions.</br>
Note that this website already includes the forward slashes for you.</br>

## Author

If you have any questions about this projects,</br>
please contact me directly at stellasunmail@gmail.com;</br>
You can view more of my projects at https://github.com/Shuyu-Sun</br>
