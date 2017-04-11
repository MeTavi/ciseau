Ciseau
------

Word and sentence tokenization in Python.

[![PyPI version](https://badge.fury.io/py/ciseau.svg)](https://badge.fury.io/py/ciseau)
[![Build Status](https://travis-ci.org/JonathanRaiman/ciseau.svg?branch=master)](https://travis-ci.org/JonathanRaiman/ciseau)
![Jonathan Raiman, author](https://img.shields.io/badge/Author-Jonathan%20Raiman%20-blue.svg)

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE.md)


Usage
-----

Use this package to split up strings according to sentence and word boundaries.
For instance, to simply break up strings into tokens:

```
tokenize("Joey was a great sailor.")
#=> ["Joey ", "was ", "a ", "great ", "sailor ", "."]
```

To also detect sentence boundaries:

```
sent_tokenize("Cat sat mat. Cat's named Cool.", keep_whitespace=True)
#=> [["Cat ", "sat ", "mat", ". "], ["Cat ", "'s ", "named ", "Cool", "."]]
```

`sent_tokenize` can keep the whitespace as-is with the flags `keep_whitespace=True` and `normalize_ascii=False`.

Installation
------------

```
pip3 install ciseau
```

Testing
-------

Run `nose2`.
