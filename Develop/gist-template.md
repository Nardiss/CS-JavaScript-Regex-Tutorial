
# Regular expressions 
 Regular expressions (RegEx) are a convenient technique used in many programming languages ​​to match certain character combinations. Rather than being limited to single or "literal" queries, RegEx allows programmers to search for any version of a string that matches a pattern. For example, in a huge database with many e-mail address entries,  a regular expression pattern search for [any name]@[any domain] [any extension] will quickly find all e-mail addresses. 
 Regular expressions are not only effective search tools, they can also be used to check formatting (such as passwords and email addresses), perform quick replaces, and aid in string splitting. 

## Summary

This core introduces JavaScript regular expressions by matching  email addresses against the following RegEx. 
 /^([a-z0-9_\.-]+) 
 @([\da-z\.-]+)\.([a-z\.]{2,6}) 
 $/ 
 Divide the regular expression into components and comment each one.

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
Boundaries
 The anchor and $ indicate that no other characters, including spaces, should be included before or after the search pattern in the regular expression that matches email addresses. Also note that all regular expression searches start and end with a  slash (/). 
 Anchors are unique characters that indicate the location of the content you are looking for. A dollar sign ($) indicates the end of the string and a caret anchor () indicates the beginning. The start or end of a word is indicated by a word boundary anchor (b). Without anchors, RegEx looks for a recognized pattern anywhere within the specified string.

 Example 
  RegEx doesn't care about position in the string, so it returns "that hat" with both occurrences of the letter combination "hat". Searching /hat$/ for "this hat" will only match "hat" at the end of the string. Also, /hat/ does not return any results because the pattern "hat" is not seen at the beginning of the string. Finally, surround the regex search with word boundaries (/bhat/) to find only instances of the word "hat".


### Quantifiers
A quantifier that counts the number of occurrences of a literal character or character before it in a set of characters is the last clause. As shown in the example below, in the email regular expression, ([...]+)@([...]+). ([. .. ]2,6. Indicates a match for any character that appears at least once in the  
 Example. 
 The email "0607tc0de@email.com" matches the regex search for /[a-z]d],8@email.com but not "ilove2code@email.com". The latter local part is 10 characters long and does not follow the quantifier specification.

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
