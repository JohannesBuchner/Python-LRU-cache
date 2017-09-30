# Introduction

It's often useful to have an in-memory cache. Of course, it's also desirable not to have the cache grow too large, and cache expiration is often desirable.

This module provides such a cache.

For the most part, you can just use it like this:

One can also create an `LRUCacheDict` object, which is a python dictionary with LRU eviction semantics:

```python
d = LRUCacheDict(max_size=3)
d['a'] = 1
d['b'] = 1
d['c'] = 1
print d['a'] # KeyError
```

## Installation

```bash
pip install simplelrucache
```

