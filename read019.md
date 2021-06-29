# Python Regular Expression


Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not. If you've ever used search engines, search and replace tools of word processors and text editors - you've already seen regular expressions in use. They are used at the server side to validate the format of email addresses or passwords during registration, used for parsing text data files to find, replace, or delete certain string, etc. They help in manipulating textual data, which is often a prerequisite for data science projects involving text mining.

In Python, regular expressions are supported by the re module. That means that if you want to start using them in your Python scripts, you have to import this module with the help of import:

```
import re
```


The re library in Python provides several functions that make it a skill worth mastering. You will see some of them closely in this tutorial.


**Basic Patterns: Ordinary Characters**


You can easily tackle many basic patterns in Python using ordinary characters. Ordinary characters are the simplest regular expressions. They match themselves exactly and do not have a special meaning in their regular expression syntax.



Examples are 'A', 'a', 'X', '5'.


Most alphabets and characters will match themselves, as you saw in the example.


The match() function returns a match object if the text matches the pattern. Otherwise, it returns None. The re module also contains several other functions, and you will learn some of them later on in the tutorial.

For now, let's focus on ordinary characters!


Do you notice the r at the start of the pattern Cookie?


This is called a raw string literal. It changes how the string literal is interpreted. Such literals are stored as they appear.

For example, \ is just a backslash when prefixed with an r rather than being interpreted as an escape sequence. You will see what this means with special characters. Sometimes, the syntax involves backslash-escaped characters, and to prevent these characters from being interpreted as escape sequences; you use the raw r prefix.



[abc] - Matches a or b or c.


[a-zA-Z0-9] - Matches any letter from (a to z) or (A to Z) or (0 to 9).


\ - Backslash. Perhaps, the most diverse metacharacter!!


If the character following the backslash is a recognized escape character, then the special meaning of the term is taken.


Else if the character following the \ is not a recognized escape character, then the \ is treated like any other character and passed through.


\ can be used in front of all the metacharacters to remove their special meaning.


There is a predefined set of special sequences that begin with '' and are also very helpful when performing search and match. Let's look at some of them up close...


\w - Lowercase 'w'. Matches any single letter, digit, or underscore.


\W - Uppercase 'W'. Matches any character not part of \w (lowercase w).


\s - Lowercase 's'. Matches a single whitespace character like: space, newline, tab, return.


\S - Uppercase 'S'. Matches any character not part of \s (lowercase s).


\d - Lowercase d. Matches decimal digit 0-9.


\D - Uppercase d. Matches any character that is not a decimal digit.


The + symbol used after the \d in the example above is used for repetition. You will see this in some more detail in the repetition section later on...


\t - Lowercase t. Matches tab.


\n - Lowercase n. Matches newline.


\r - Lowercase r. Matches return.


\A - Uppercase a. Matches only at the start of the string. Works across multiple lines as well.


\Z - Uppercase z. Matches only at the end of the string.


\b - Lowercase b. Matches only the beginning or end of the word.