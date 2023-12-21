##  Regex matching Hex value
## Summary

This application will breaking down the components of a expression used to match Hex Values. Hexadecimal code is user to describe color to a coputer. Cause computers are sometimes dumb and don't like "red". A hexadecimal color is a six-digit code starting with a # sign.  /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Bracket Expressions](#bracket-expressions)
- [The OR Operator](#the-or-operator)

## Regex Components

## Anchors
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
Anchors do not match any character but they match a position after, before, or between characters. They can be used to “anchor” at a certain position. The caret ^ matches the position before the first character in the string, ^a to abc matches a but ^b does not match abc at all, because the b can't be matched right after the start of the string, matched by ^.$ matches right after the last character in the string. c$ matches c in abc, a$ does not match at all.

## Quantifiers
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
Quantifiers are used to show how many characters as well as how many instances of a group, character or class must be present for a correct match. The characters ",+,?,{}" are considered quantifiers. The ? will match 0 or 1 time.  The Hex Value has {6} (Hex Triplet Format) and {3} (Shorthand Hex Format), this shows that the length of the component should be 6 for {6} and 3 for {3}.

## OR Operator
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
The "or" operator within a is defined using | . The or operator shows that it could be either of the components that are being separated as define with the | element. For our hex value regular expression we have ([a-f0-9]{6}``|``[a-f0-9]{3}).  The hex value could be 6 characters [a-f0-9]{6} or 3 characters [a-f0-9]{3}.

## Character Classes
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
Character classes are components that tells us what type of characters to expect that could be defined with []. a-f searches for letters a-f and 0-9 searches for digits 0-9.

## Bracket Expressions
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
Matches any character in the square brackets. For example [nN] [oO] matches no, nO, No, and NO. gr[ae]y matches both spellings of the word 'grey'; that is, gray and grey.

## Author

Joe(y) Gaytan
Profile - https://github.com/Jo3yG/Challenge02.git
Github - https://github.com/Jo3yG
