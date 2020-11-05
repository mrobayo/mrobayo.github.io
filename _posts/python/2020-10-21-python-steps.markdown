---
layout: single
title:  "Python Steps"
date:   2020-10-20 11:00:00 -0500
categories: python
---

### Replace multiple spaces in a string

```python
  message = 'the    way,    and the   truth, and the life'
  print( re.sub(' +', ' ', message) )

#=> the way, and the truth, and the life
```




implement a function that will turn the old-style syntax into a new one. Implement a function that will turn the old-style string formating s into a new one so that the following two strings have the same meaning:

s % (*args)
s.format(*args)
Example

For s = "We expect the %f%% growth this week", the output should be
newStyleFormatting(s) = "We expect the {}% growth this week".


import re
    
def newStyleFormatting(s):
    return re.sub('\%[\%a-z]',lambda m:'%'if m.group()=='%%'else'{}', s)
