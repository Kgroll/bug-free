# Powerful Password Matcher

Welcome to Powerful Password Matcher!!  
If you follow the criteria given, it will allow you to validate a unique and powerful password.  
In order to test your passwords validity, copy the regex code and paste it in a regex tester (eg: https://regexr.com/) then enter your chosen password.  
If your password meets the criteria you will be certain to have a great password!   
Be creative but don't forget to create something you can easily remember!!  

## Summary

The regex I am describing is for creating and validating a strong password by meeting the following criteria
- must include at least 8 and up to 20 characters
- must include at least one upper case letter
- must include at least one lower case letter
- must include at least one digit
- must include at least one special character


`/^(?=.*?[A-Z])(?=.*?[a-z])(?=.*?[0-9])(?=.*?[#?!@$ %^&*-]).{8,21}$/`


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Lazy Match](#lazy-match)
- [Look-ahead](#look-ahead)

## Regex Components

### Anchors
`/` This denotes the beginning of a regular expression paragraph

`^` Denotes the beginning of the line
`$` Denotes the end of the line

### Quantifiers
`*` Assesses the preceding tokens to match 0 or more of the criteria  
`{8,21}` Matches the number of characters in the preceding tokens 

### Character Classes
`[]` Are used to define a character class  
`.` Matches any single character except a new line  
`[A-Z]` Matches upper case letters  
`[a-z]` Matches lower case letters  
`[0-9]` Matches digits between 0 and 9  
`[#?!@$ %^&*-]` Matches the listed special characters  

### Grouping and Capturing
`()` Parentheses are used to place a particular part of a regex in order so they can group that part of the regex together,   
   this also captures the information within the parentheses

### Bracket Expressions
`{}` Are used to specify the exact amount of things to match  
   used here to determine the minimum and maximum length of the password: {8,21} where 8 is the minimum and 21 is the maximum  
`[]` Are used to define a character class  
`()` Parentheses are used to place a particular part of a regex in order so they can group that part of the regex together,   
   this also captures the information within the parentheses  

### Lazy Match
`?` Denotes the lazy match allowing the preceding quantifier, in this case *, to match as few characters as possible 

### Look-ahead
`(?= plus the group or character class)` This allows a  search for the character or characters in that particular group or class,  
if the character is present then the regex recognizes the match and if it is not it rejects it  
   (Look-behind `(?<=)` could also be used however it is not recognized in all languages so I did not include it in my regex)  
   
## Author
Created by Kristen Groller  
I am presenting enrolled in the U of T Coding bootcamp.   
I hope this gist helps you validate a powerful password.  
Github link https://github.com/Kgroll
