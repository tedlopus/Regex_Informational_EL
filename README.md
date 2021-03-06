# Regex_Informational_EL
A deeper dive into regular expressions and how they work. This is an informational guide for JavaScript regular expressions and what exactly "regular expression" means. Please enjoy this read.

## Summary
A regular expression in JavaScript are patterns used to match character combinations in strings. Regular expressions can also be objects which can be constructed one of two ways. The first way to create regular expressions is by usind literal notation. The literal notation parameters are enclosed within slashes. The other way to create regular expressions is by using a constuctor. The constructor's function parameters are enclosed with quotations. As we continue to disect regex, we will be using /word/ as our base example. Each section of this will use this example to clearly show the topic being discussed. The regex I will be using for this will be "\A[a-zA-Z][a-z\d][\w][\D]\s(?:%%%)a+(?i:run|walk)\n".

## Table of Contents
* [Anchors](#Anchors)
* [Quantifiers](#Quantifiers)
* [Grouping Constructs](#Grouping_Constructs)
* [Bracket Expressions](#Bracket_Expressions)
* [Character Classes](#Character_Classes)
* [The OR Operator](#The_OR_Operator)
* [Flags](#Flags)
* [Character Escapes](#Character_Escapes)
* [License](#License)
* [Questions](#Questions) 
  
## Anchors
\A is the part of this regex that is an anchor. This anchor matches the start of the string and is not affected by multiline mode. This starting string anchor is attached to [a-zA-Z] which means the starting character of the string could be any lowercase or uppercase letter of the alphabet.

## Quantifiers
a+ is the part of this regex that is a quantifier. This quantifier matches one or more consecutive 'a' characters. This can be 'a', 'aa', 'aaa', 'aaaa', etc. This quantifier stands alone in the regex and focuses only on 'a'.

## Grouping_Constructs
There are two examples of grouping constructs in this regex. They are (?:%%%) and (?i:run|walk). I will focus on (?:%%%) for this portion of the informational regex. (?:...) is a non-capturing group that allows you to apply quantifiers to part of your regex but does not capture an ID. This grouping construct matches everything that is enclosed in the parentheses and follows '?:'.

## Bracket_Expressions
[a-z\d] is one part of this regex that is a bracket expression. This bracket expression matches any characters between lowercase a and z and also matches any digit with '\d'. These bracket expressions allow you to list possible matches for one chracter entry within the brackets.

## Character_Classes
[\w] is one part of this regex that is a character class. The '/w' is a special character class because it can match any alphanumeric character including underscore. It is equivalent to the following bracket expression: [A-Za-z0-9_].

## The_OR_Operator
(?i:run|walk) is the part of this regex that is the OR operator. The OR operator in this regex ( | ) is similar to the OR operator in javascript expressions ( || ). The OR operator in this grouping construct matches to either run or walk.

## Flags
(?i:run|walk) conatins the flag part in this regex. 'i' is a case-insensitive search that accepts either uppercase or lowercase versions of run or walk since it is combined with the previously mentioned OR operator.

## Character_Escapes
There are many character escape sequences for regular expressions but I choose /n for mine. '/n' creates a new line and matches when a new line is entered. It can be used with multiline, not single line, expressions.

## License
This project is licensed under  MIT.
Read more about [MIT](https://opensource.org/licenses/MIT).

## Questions
Find me Github: 
[Ted Lopus](https://github.com/tedlopus)