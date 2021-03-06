Python case insensitive dictionary
==================================
.. image:: https://img.shields.io/pypi/v/CaseInsensitiveDict.svg
.. image:: https://img.shields.io/pypi/wheel/CaseInsensitiveDict.svg
.. image:: https://api.travis-ci.org/tivvit/python-case-insensitive-dict.svg?branch=master
.. image:: https://img.shields.io/github/license/tivvit/python-case-insensitive-dict.svg

* implements all standard dictionary methods
* supports nested dicts
* this implementation does not preserve original key case

Install
~~~~~~~

.. code-block:: python

    pip install CaseInsensitiveDict

Example
~~~~~~~

.. code-block:: python

    from CaseInsensitiveDict import CaseInsensitiveDict

    cid = CaseInsensitiveDict({"A": {"A": 1}, "B": 2, "c": 3})

    print cid["A"] # >>> {'a': 1}
    print cid["a"] # >>> {'a': 1}
    print cid["A"]["a"] # >>> 1
    print cid["b"] # >>> 2
    print cid["C"] # >>> 3

Development
~~~~~~~~~~~

Feel free to contribute.

Copyright and License
~~~~~~~~~~~~~~~~~~~~~
2015 `Vít Listík <http://tivvit.cz>`_

Released under `MIT licence <https://github.com/tivvit/python-case-insensitive-dict/blob/master/LICENSE>`_