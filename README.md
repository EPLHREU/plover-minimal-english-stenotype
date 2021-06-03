# Minimal English Stenotype

> Plover system plugin with no automatic unfolding of orthography rules

One normally helpful feature of plover is it's ability to automatically unfold certain suffixes from a stroke. 
This allows plover to recognise more condensed strokes for words that may not exist in the dictionary.

For example, if plover had a dictionary containing only the following entries:
``` json
"CAT" : "cat",
"-G" : "{^ing}",
```

One could stroke `KAT` to produce "cat", or `KAT/-G` to produce "cating".
However, plover would also recognise `KAGT` producing "catting".

This may not be wanted, especially when using plover with other theories such as Magnum or Pheonix, as it can lead to output that is unrelated to what is expected.

This plugin removes all of these additional systems for english stenotype, allowing plover to only type entries clearly defined in the dictionaries present. 

## Installation

Install from the Plover plugin manager.
