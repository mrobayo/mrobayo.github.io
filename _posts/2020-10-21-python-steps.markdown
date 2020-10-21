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



