# Regular Expression with Python

### Importing the required module
```python
import re
```

### The texts and patterns to work upon
```python
text_to_search = """
abcdefghijklmnopqurtuvwxyz
ABCDEFGHIJKLMNOPQRSTUVWXYZ
1234567890

Ha HaHa

MetaCharacters (Need to be escaped):
.[{()\^$|?*+

coreyms.com

321-.555-4321
123.555.1234

Mr. Schafer
Mr Smith
Ms Davis
Mrs. Robinson
Mr. T
"""

sentence = "start a sentence and then bring it to an end"
```

### Pattern to match
```python
pattern = re.compile("abc")
```

### How to match
```python
matches = pattern.finditer(text_to_search)

for match in matches:
    print(match)
    
# OUTPUT: <_sre.SRE_Match object; span=(1, 4), match='abc'>

print(text_to_search[1:4])
# OUTPUT: abc
```

### Python File
[Click Here](../py/regex.py)