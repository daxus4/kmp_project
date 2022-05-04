# KMP Project

Pattern-matching (PM) algorithms can find occurrences of a pattern string (P) in another string (S), which is usually orders of magnitude longer.
With the advent of bioinformatics, the need for PM algorithms that can work in linear time and memory complexity increased because there are applications that require to match multiple patterns on massive strings, for example the entire human genome. Knutt, Morris and Pratt developed a PM algorithm, often called KMP in literature, that, by building an index of P, has linear time and memory performance [1].
In this project I reproduced the algorithm in Python and then implementing a parallel version that split S in overlapped substring and can run an instance of KMP on each substring. The substrings are overlapped because occurrences of the pattern can be found straddling two strings and only if those two string overlap with a determined number of character this algorithm can work correctly.
 I tested both the standard and the parallel version, with particular attention when I was dealing with the problem mentioned above.

[1] Knuth, Donald; Morris, James H.; Pratt, Vaughan (1977). "Fast pattern matching in strings". SIAM Journal on Computing. 6 (2): 323–350. CiteSeerX 10.1.1.93.8147. doi:10.1137/0206024.

