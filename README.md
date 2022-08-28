# Chooser Cap

Chooser option on interest forward rates may also be called chooser cap and chooser floor, respectively. A cap (floor) is a portfolio of caplets (floorlets). For a given number k, a chooser cap (floor) is an option which entitles the option owner the right to exercise at most k caplets (floorlets) out of the total n caplets (floorlets). 

As European and Bermudan options are standard products, a so-called k-out-of-n (or simply (k/n)-) Bermudan option is also a standard product in the derivative market. A chooser option is an example of (k/n)-Bermudan option. Bermudan option is a type of callable exotics (see https://finpricing.com/lib/EqCallable.html)

A chooser cap (floor) is different from the traditional European/Bermudan option that the owner of the chooser option has multiple chances to exercise. The rigorous definition of chooser option is given in the appendix section of this report. From the definition of the chooser option, a lower bound of the value of the chooser cap (floor) is the sum of first k maximal values of (European) caplets (floorlets). To get a good upper bound is not trivial.

Similarly, the function σ(·) is also an interpolated function of t given by {(ti, σi)} where σi is the implied volatility of the ith caplet (floorlet).

From a rigorous view point, the dynamics may not be completely arbitrage-free. However, it perfectly re-produces all European caplets (floorlets) market prices automatically. Therefore, the dynamics can be considered as approximately arbitrage-free without any additional calibration. It should also be noted that volatility skewness is not considered in this dynamics.

A tree approach is applied. The feature of multiple exercise makes the backward procedure more complicated

Let {Xt } be the underlying strictly positive rate of a derivative which is to be considered. Let T (T > 0) be a given number, n and k be given integers. Let T = {T1, · · · , Tn} be a given set of possible exercise time points, where 0 _ T1 < · · · < Tn = T. Let T be a set of stopping times on T which satisfies some technical conditions. Let f be a given function.

With the given above, a so-called k-out-of-n (or (k/n)-) Bermudan option, which is corresponding to (X,T,T , k, f), is a derivative security which provides the total payoffs made up to and including time 

Particularly, if 1 = k < n, the derivative reduces to a conventional Bermudan option with n possible exercise time points in T. If k = n, then it becomes the sum of n European options with maturities corresponding to each term in T. If, further, k = n = 1, then it leads to a conventional European option matured at T1.

Without the loss of generality, let t = 0 be the valuation time with known value of X0. Suppose that a tree of the underlying X, denoted by X , has been built which is rooted at (0,X0) and is ended at time of T.


