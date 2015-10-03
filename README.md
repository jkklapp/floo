# floo
Provide a set of symbols and sequence them.

Floo is a small python library that given a sequence of symbols, provides order on them and basic arithmetic operations.

# Easy example

Consider the set of symbols S = {'a', 'x', '?', '3'}. Let's create a Floo instance with it.

```
from floo import Floo

# Create a Floo instance with a set of symbols. The symbols have the order provided in the input.
>>> f = Floo("ax?3")
```
We can initialize a counter for our set.
```
>>> i = f.initial()
>>> i
'a'
```
We can increment our counter.
```
>>> f.inc(i)
'x'
```
Operations can be made with well-formed words of our set of symbols. Let's sum 'a3??x' and '3??xx'.
```
>>> f.sum('a3??x', '3??xx')
'xaaaaa'
```



