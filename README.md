# Regextutorial
Tutorial: Describe Hex Values(Regex)

Regular Expressions. A regex is composed of a combination or pattern of simple(literal) characters or meta characters. Literal characters are numbers and letters. Meta characters are twelve special characters you can find on your keyboard.Meta characters are normally used to find a wider set of characters. These patterns and/or combinations are used in coding and algorithems.This helps the code or algorithm find certain combinations and/or patterns within strings. To either replace, delete, modify or validate data within a string.

For example:

Standard format

Red = #FF0000

Green = #008000

Blue = #0000FF

Shorthand format

Red = #f00

Lime = #0f0

Blue = #00f

note: not all colors can be put in shorthand format

Below you'll see the regex for hex values.

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

I will break down these values in this tutorial for the reader to better understand the use of this type of regex. By the end of this tutorial the reader will have an understanding of how the anchors, quantifiers, OR operator, characters classes, and bracket expressiongs function within the context of regex hex values.

Table of Contents:
Anchors
Quantifiers
Grouping Constructs
The OR Operator
Character Classes
Author
Regex Components
Below is a list of the components and terminology.

Anchors:
The anchors in this set of regex are ^ and $.

They're considered meta characters. The ^ is known as a carat, hat, circumflex, or exponent symbol. The $ is known as the dollar sign.

The ^ represents the beginning of string or a line, and the $ represents the end of a string or a line. For example: ^789 will match any line or string that begins with 789. The same goes with $ but instead it is placed at the end. Example: 123$ will match any line or string that ends with 123.

Quantifiers:
The quantifiers in this set of regex are a question mark( ? ), and curly brackets with numbers inside of them. Such as {6} and {3}.

Quantifiers are used in code and algorithems to communicate how many characters are expected. Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found.The ? plays the role of a conditional in regex. The ? matches any previous character 0 or 1 times. The number between the curly brakets indicates the length of the hex code you are looking for. The {6} is used for standard format(Hex Triplet Format) and {3} is used for shorthand format.

Examples of these are in the summary section.

Grouping Constructs:
The grouping constructors are ([a-f0-9]{6}|[a-f0-9]{3}). These grouping constructors are composed of bracket expressions that group what specifications of what you want your code or algorithm to look for. The bracket expressions are open and closed parenthesis( () ), open and closed brackets( [] ), open and closed curly brackets( {} ), and a pipe/verticle bar ( | ). More infomation on how the | functions within theses grouping constructors will be seen in the OR operator section.

The OR Operator:
The OR operator is a pipe/verticle bar ( | ).

This meta character | is placed between [a-f0-9]{6} and [a-f0-9]{3} enclosed by parenthesize. As the name indicates; this special character is inserted in the middle of two bracket expressions to indicate that the code or alrorithem should look for what is defined within the two bracket expressions. In the context of hex values it permits for your code or algorithem to look for standard format {6} or shorthand format {3}.In general it's interpreted as an and statement.

Character Classes:
The character classes of this regex are [a-f0-9].The definitions for these characters and meta characters are seen in the above sections. The only new one in this reqex is this symbol (-). Better known as a hyphen,minus, or dash.

Character classes are components within our regex that tells the code or algorithem what type of characters to expect. In our example our character classes are within brackets [] followed by the quantifiers. [a-f0-9] creates the parameters for a search. a-f searches for letters athough f and 0-9 searches for digits 0 through 9.

Author Randy 
