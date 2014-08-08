Test Cases for Rivest Sampling Algorithm
========================================

The purpose of this repository is to provide test cases for a
pseudo-random sampling algorithm described by [Ronald L. Rivest][rivest].
This algorithm was designed for things like selecting precincts
at random for an election audit.

The [reference implementation][ref-impl] of the algorithm
(written in Python), along with a description of the algorithm,
can be found on Rivest's web site.  [Philip B. Stark][stark]
also has an online [browser implementation][browser-impl] on his web site.

The test cases in this repository can be used to help check that additional
implementations are correct.

The test cases were checked using Python 2.6.9 and the reference
implementation downloaded from Rivest's web site on August 8, 2014.
(The implementation states that it was checked using Python 2.6.7.)
For convenience, we have included a copy of the downloaded implementation
in this repository.  It is the file [sampler.py](sampler.py).


[browser-impl]: http://www.stat.berkeley.edu/~stark/Java/Html/sha256Rand.htm
[ref-impl]: http://people.csail.mit.edu/rivest/sampler.py
[rivest]: http://people.csail.mit.edu/rivest/
[stark]: http://www.stat.berkeley.edu/~stark/
