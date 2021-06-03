# Minimal English Stenotype

> Plover system plugin with no automatic unfolding of orthography rules

One normally helpful feature of plover is it's ability to automatically unfold certain suffixes from a stroke. 
This allows plover to recognise more condensed strokes for words that don't exist in the dictionary.

For example, if plover had a dictionary containing only the following entries:
``` json
"CAT" : "cat",
"-G" : "{^ing}",
```

One could stoke the following:
- `KAT` -> "cat"
- `KAT/G` -> "catting" using normal plover orthography rules for suffixes
- `KAGT` -> "catting" using plover automatic unfolding orthography rules

This final method may not be wanted, especially when using plover with other theories such as Magnum or Phoenix, as it can lead to output that is unrelated to what is expected and does not have an entry.
This can make finding unassigned brief strokes more difficult, as you would have to search specifically through the dictionary rather than seeing untranslated raw steno output.
Additionally, this can trip up the creation of briefs, especially in briefs heavy theories as they may not follow the same ideas that plover does.

This plugin removes this automatic unfolding orthography from plover, allowing it to exactly follow entries specified in dictionary. 

## Installation

Install from the Plover plugin manager.
