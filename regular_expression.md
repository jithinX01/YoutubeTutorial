## Regular expression or Pattern Matching for beginners

#### A regular expression is a pattern that describes a set of strings.

#### uses in grep, or any pattern matching in programming.

#### Any single character

```perl
. #dot or period  Matches any character other than newline
```

#### Any White space character

```perl
\s #Matches any space, tab or newline character.
```

#### Any Non White space character

```shell
\S #Matches anything other than a space, tab or newline.
```

#### Any digit

```shell
\d #Matches any decimal digit
```

#### Any non digit

```shell
\D #Matches anything other than a decimal digit.
```

#### Any word character

```shell
\w #Matches any letter, digit or underscore
```

#### Any non word character 

```shell
\W #Matches anything other than a letter, digit or underscore.
```

#### Zero or one of

```perl
a?  #Matches an `a` character or nothing. 
```

#### Zero or more of

```perl
a* #Matches zero or more consecutive `a` characters.
.* #matches zero or more of any characters, matches everything.
```

#### One or more of

```perl
a+ #Matches one or more consecutive `a` characters.
```

#### Start of a string

```perl
^ #Matches the start of a "string" without consuming any characters
^bc #matches bc, not abc
```

#### End of a string

```perl
$ #Matches the end of a "string" without consuming any characters
ab$ #Matches ab, not abc
```

#### A character in the range

```perl
[a-z] #Matches any characters between a and z, including a and z
[0-9] # Matches any decimal digit same as \d
```

#### A single character of

```perl6
[abc] #Matches either an a, b or c character
[a-zA-Z0-9_] #Matches any letter, digit or underscore Equivalent to \w
```

#### A character except

```perl6
[^abc] #Matches any character except for an a, b or c
```

#### Match either  or 

```shell
(a|b) #Matches the a or the b part of the subexpression.
^a|bc$ # matches a character start with a or ends with bc. aa matches, cbc matches, abc matches
```

#### Exactly of n number of

```shell
a{3} #Matches exactly 3 consecutive `a` characters.
```

#### n or more number of

```shell
a{3,} #Matches at least 3 consecutive `a` characters.
```

#### Between n and m number of 

```shell
a{3,6} #Matches between 3 and 6 (inclusive) consecutive `a` characters
```

#### A word boundary

```shell
\b
#Matches, without consuming any characters, immediately between a character matched by \w and a character not matched by \w (in either order). It cannot be used to separate non words from words.
d\b # in string "word boundary word boundaries are odd", matches 'd' in "word" and "odd" 
```

#### A non-word boundary 

```shell
\B
#Matches, without consuming any characters, at the position between two characters matched by \w.
r\B # in string "regex is really cool", matches 'r' in "regex" and "really"
```

#### Capture everything enclosed.

```shell
(ab)
#Parts of the regex enclosed in parentheses may be referred to later in the expression or extracted from the results of a successful match, This is mostly used for match and replace situations
(ab).* # ab captured in group 1. matching a string "abcbab" , "ab" captured as $1.
/(ab).*/$1_/ # matches "abcbab" and capture ab in $1, resulting string after replace will be "ab_"

```

###### Ref:

[regex 101](https://regex101.com/)

```shell
man grep
```

