# Regex Tutorial

----------


This Regex (regular expression) Tutorial is created to help undestand and define a specific regex. A regex being a sequence of characters that defines a specific pattern that can be used for searching, validation, parsing/replacing strings and passing through translating data to other formats. A regex is extremely useful in extracting information from any text by searching for the specific pattern. As well this tool can be used in almost all programming languages JavaScript, Java, VB, C #, C / C++, Python, Perl, Ruby, Delphi, R, Tcl, and many others.

----------

## Summary

----------


HTML Tag Regex

/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/
* [HTML](#HTML)

An HTML tag is a piece of markup language used to indicate the beginning and end of an HTML element in an HTML document. A tag tells the browser to do something and are inclosed in less than (<) and greater than (>) signs. For every opening tag, a closing tag is used containing the code within to execute.

----------


### Table of Contents
* [Anchors](#Anchors)
* [Quantifiers](#Quantifiers)
* [OROperator](#OROperator)
* [CharacterClasses](#CharacterClasses)
* [Flags](#Flags)
* [GroupingandCapturing](#GroupingandCapturing)
* [BracketExpressions](#BracketExpressions)
* [GreedyandLazyMatch](#GreedyandLazyMatch)
* [Boundaries](#Boundries)
* [Back-references](#Back-references)
* [Look-aheadandLook-behind](#look-aheadandLook-behind)
* [Author](#Author)

----------


#### Anchors
The characters ^ and $ are both considered to be anchors.

###### HTML Tag Regex 
^ Matches the beginning of the string, or the beginning of a line if the multiline flag (m) is enabled. < This matches a position, not a character. $ Matches the end of the string, or the end of a line if the multiline flag (m) is enabled. This matches a position, not a character.

---------

#### Quantifiers
Quantifiers set the limits of the string that your regex matches. 

###### HTML Tag Regex 
+ is used in group 1, 2 and 3. The + quantifier matches the pattern one or more times. Also the * is used in group 3 as well. The * quantifier matches the pattern zero or more times.

---------

#### OR Operator
Acts like a boolean OR. Matches the expression before or after the |. It can operate within a group, or on a whole expression. The patterns will be tested in order.

###### HTML Tag Regex  
| is used in group 3.

---------

#### Character Classes
A character class in a regex defines a set of characters, any one of which can occur in an input string to fulfill a match. Common character classes:
. matches any character except the newline character.
\d matches any Arabic numeral digit. This class is equivalent to the bracker expression [0-9].
\w matches any character that is not a word character (alphanumeric and underscored) such as [A-Za-z0-9_].
\s matches a single whitespace character, including tabs and line breaks.

###### HTML Tag Regex  
\s Matches any whitespace character (spaces, tabs, line breaks).

---------

#### Flags
Flags are placed at the end of a regex, after the second slash, and they define additional functionality or limits for the regex. There are six optional flags that can be used, either separately or together and in any order. Most common flags are:
g—Global search: the regex should be tested against all possible matches in a string.
i—Case-insensitive search: case should be ignored while attempting a match in a string.
m—Multi-line search: a multi-line input string should be treated as multiple lines.

No Flags are used in HTML tag regex.

---------

#### Grouping and Capturing
Grouping constructs have two primary categories: capturing and non-capturing. The primary way you group a section of a regex is by using parentheses (()). Each section within parentheses is known as a subexpression. The important thing to understand is that capturing groups capture the matched character sequences for possible re-use (including a numbered backreference) while non-capturing groups do not.

###### HTML Tag Regex  
3 () Groups multiple tokens together and creates a capture group for extracting a substring or using a backreference.

---------

#### Bracket Expressions
Anything inside a set of square brackets ([]) represents a range of characters that we want to match. These patterns are known as bracket expressions, but they are also known as a positive character group, because they outline the characters we want to include.

###### HTML Tag Regex  
2 [] Matches a character having a character code between the two specified characters inclusive.

---------

#### Greedy and Lazy Match
The quantifiers ( * + {}) are greedy operators, so they expand the match as far as they can through the provided text.
The opposite ? when implemented, makes the preceding quantifier lazy, permitting it to match as few times as possible.

###### HTML Tag Regex  
Only {} are not used.

----------

#### Character Escapes
The backslash (\) in a regex escapes a character that otherwise would be interpreted literally. For example, the open curly brace ({) is used to begin a quantifier, but adding a backslash before the open curly brace (\{) means that the regex should look for the open curly brace character instead of beginning to define a quantifier. This is common when looking for strings with special characters that are the same as a particular component of a regex. It's important to note that all special characters, including the backslash (\), lose their special significance inside bracket expressions.

###### HTML Tag Regex  
\/ Matches a "/" character (char code 47).

---------

#### Boundaries
Boundries such as \b and \B represent an anchor like caret (it is similar to $ and ^) matching positions where one side is a word character (like \w) and the other side is not a word character. For instance it may be the beginning of the string or a space character. \B matches all positions where \b doesn’t match and could be if we want to find a search pattern fully surrounded by word characters.

---------

#### Back-references
The backreference \1 references the first capturing group. \1 matches the exact same text that was matched by the first capturing group. The / before it is a literal character. It is simply the forward slash in the closing HTML tag that we are trying to match.

###### HTML Tag Regex  
\1 Matches the results of a capture group. For example \1 matches the results of the first capture group & \3 matches the third.

----------

#### Look-ahead and Look-behind
Lookahead and lookbehind, collectively called “lookaround”, are zero-length assertions just like the start and end of line, and start and end of word anchors explained earlier in this tutorial. The difference is that lookaround actually matches characters, but then gives up the match, returning only the result: match or no match.

(?=foo)-Lookahead-Asserts that what immediately follows the current position in the string is foo.
(?<=foo)-Lookbehind-Asserts that what immediately precedes the current position in the string is foo.
(?!foo)-Negative Lookahead-Asserts that what immediately follows the current position in the string is not foo.
(?<!foo)-Negative Lookbehind-Asserts that what immediately precedes the current position in the string is not foo.

----------

#### Author
Joshua Pace

Any questions? You can contact me directly at jwputah7@gmail.com

Or visit my [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/jwputah)