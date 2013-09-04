[←](../) Best Practice
======================

> A best practice is a method or technique that has consistently shown results
> superior to those achieved with other means, and that is used as a benchmark.
> In addition, a "best" practice can evolve to become better as improvements are
> discovered.
> ~ [Wikipedia][1]


General
-------

* Document everything. There is no such thing as too much documentation.
* Don't duplicate the functionality of a built-in library.
* Don't swallow exceptions or "fail silently".
* Don't write code that guesses at future functionality.
* [Exceptions should be exceptional][2].
* [Keep the code simple][3].


Git
---

* Use global ignore config file [(Why?)][6]
* Don't commit private data [(remove it!)][7]


Versioning
----------

* Use [Semantic Versioning][8]


Object-Oriented Design
----------------------

* Avoid global variables.
* Avoid long parameter lists.
* Limit collaborators of an object (entities an object depends on).
* Limit an object's dependencies (entities that depend on an object).
* Prefer composition over inheritance.
* Prefer small methods. Between one and five lines is best.
* Prefer small objects with a single, well-defined responsibility. When an
  object exceeds 100 lines, it may be doing too many things.


Database
--------

* Prefer MySQL
* Prefer [InnoDB Storage Engine][5] (if using MySQL)
* Naming DB column titles by separating words with underscores `_` e.g. 
  `user_id`, `vendor_id`


Web APIs
--------

* Prefer [JSON][9].
* Prefer [RESTful implementations][10].


CSS
---

* Use [LESS][4].


Browsers
--------

* Don't support clients without Javascript.
* Don't support IE6 or IE7.


[1]: http://en.wikipedia.org/wiki/Best_practice
[2]: http://pragmatictips.com/34
[3]: http://code.mumak.net/2012/02/simple-made-easy.html
[4]: http://lesscss.org/
[5]: http://en.wikipedia.org/wiki/InnoDB
[6]: http://kingori.co/minutae/2013/04/global-ignores/
[7]: https://help.github.com/articles/remove-sensitive-data
[8]: http://semver.org/
[9]: http://www.json.org/
[10]: http://en.wikipedia.org/wiki/Representational_state_transfer#RESTful_web_APIs
