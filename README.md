Test Cases for Rivest Sampling Algorithm
========================================

The purpose of this repository is to make test cases publicly available
for the [SHA-256][sha-256] pseudo-random sampling algorithm described by
[Ronald L. Rivest][rivest] in 2011.

The test cases in this repository can be used to help check that new
implementations are correct.


Algorithm Background
--------------------

The Rivest sampling algorithm is for things like selecting precincts
at random for an election audit.

The [reference implementation][ref-impl] of the algorithm (written in Python),
along with a description, can be found on Rivest's web site.
[Philip B. Stark][stark] also has an online
[browser implementation][browser-impl] on his web site.
An AngularJS implementation called [`free-sampler`][free-sampler]
is also in progress.


Test Details
------------

The tests are located in the file [`tests.json`](tests.json).
The sample range for each test is the list of whole numbers from 1 to
the upper limit `total`.  The tests were run "allowing duplicates."

The test cases were checked using Python 2.6.9 and the
reference implementation downloaded from Rivest's web site on August 8, 2014.
(The implementation states that it was checked using Python 2.6.7.)
For convenience, we included a copy of that download in this repository
as the file [`sampler.py`](sampler.py).

The test cases were also checked using [`free-sampler`][free-sampler].


Deployment
----------

For convenience, this repository has a [`bower.json`](bower.json) file,
which lets one include the test cases in another web application
using [Bower](http://bower.io/).


License
-------

The contents of this repository are licensed under a BSD 3-clause license,
unless indicated otherwise.  See the [`LICENSE`](LICENSE) file
for the BSD license.  Note that Rivest's reference implementation,
which this repository contains a copy of, is licensed under
the MIT License and not BSD.


Author
------

Chris Jerdonek (<chris.jerdonek@gmail.com>)


[browser-impl]: http://www.stat.berkeley.edu/~stark/Java/Html/sha256Rand.htm
[free-sampler]: https://github.com/cjerdonek/free-sampler
[ref-impl]: http://people.csail.mit.edu/rivest/sampler.py
[rivest]: http://people.csail.mit.edu/rivest/
[sha-256]: http://en.wikipedia.org/wiki/SHA-2
[stark]: http://www.stat.berkeley.edu/~stark/
