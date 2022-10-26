# Gucci's Regex tutorial

## Summary

To begin Regex is similar to doing "command + f" or "cntr+f" in terms of being to able to search the document for something. The biggest difference is that with Regex or regular expressions the user can be used when you need something that's a little more broad. Regex is more-so used for pattern recognition, but can also get very specific.
I will be using a basic expression.
/([A-Z][A-Z][A-Z])\w|([A-Z][a-z])/g
(I am using this expression to pull information from this page https://www.cardboardconnection.com/2022-panini-world-cup-stickers-qatar-cards)

## Table of Contents

- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components
Regex components are as the name implies, basically ways to make a search pattern more/less specific. 

### Quantifiers
quantifiers basically specify how many times a charachter or group of characters have to happen before its actuallly selected, this is a bad as example as I unfortunately did not use one

### Grouping Constructs
grouping construct uses () in order to pull out a certain string of characters that fits the specific pattern in my case "([A-Z][A-Z][A-Z])" with this I can pull out a group if 3 upper case letters from A to Z, which I want in order to get the country code. Basically the paranthesis allow the user to find a more specific pattern by grouping together more requirements

### Bracket Expressions
Brackets help pull out characters that match the characters defined in the brackets which again in my case will either be [A-Z] or [a-z]
### Character Classes
Character classes find specific letters or a range of letters. Mine is set to look for A-Z but if I wanted only around half of the country codes I could have used ([A-M][A-Z][A-Z]), or if I wanted a specif country like Mexico, I could narrow the pattern recognition by doing ([MEX]) 
### The OR Operator
The or operator allows for users to look for multiple things at once. again in my case /([A-Z][A-Z][A-Z])\w|([A-Z][a-z])/g I have an or operator so I can pull out the country code OR players name hence why in the second grouping the first letter is capital while the second one is not.
### Flags
flags allow for a more general search for example adding an g/ will allow the user to select text that matches, multiple times instead of just once. Which I need since I have to pull the same country code multiple times


## Author

Fabian Gutierrez - https://github.com/Guccierrez?tab=repositories

