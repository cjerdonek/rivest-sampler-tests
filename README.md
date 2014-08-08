Test Cases for Rivest Sampling Algorithm
========================================

The purpose of this repository is to provide test cases for the
simple [SHA-256][sha-256] pseudo-random sampling algorithm described by
[Ronald L. Rivest][rivest].
This algorithm is especially suitable for things like selecting precincts
at random for an election audit.

The [reference implementation][ref-impl] of the algorithm (written in Python),
along with a description, can be found on Rivest's web site.
[Philip B. Stark][stark] also has an online
[browser implementation][browser-impl] on his web site.
The test cases in this repository can be used to help check that new
implementations are correct.

The contents of this repository are licensed under a BSD 3-clause license,
unless indicated otherwise.  For example, the reference implementation
was released under the MIT License.  See the [`LICENSE`](LICENSE) file
for the BSD license.


Test Details
------------

The tests are located in the file [`tests.json`](tests.json).
The sample range for each test is the list of whole numbers from 1 to
the upper limit `total`.  The tests were run "allowing duplicates."

The test cases were checked using Python 2.6.9 and the
reference implementation downloaded from Rivest's web site on August 8, 2014.
(The implementation states that it was checked using Python 2.6.7.)
For convenience, we have included a copy of the downloaded implementation
in this repository as the file [`sampler.py`](sampler.py).


[browser-impl]: http://www.stat.berkeley.edu/~stark/Java/Html/sha256Rand.htm
[ref-impl]: http://people.csail.mit.edu/rivest/sampler.py
[rivest]: http://people.csail.mit.edu/rivest/
[sha-256]: http://en.wikipedia.org/wiki/SHA-2
[stark]: http://www.stat.berkeley.edu/~stark/
