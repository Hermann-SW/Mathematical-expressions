For odd prime _p_, the difference is unique:

$$\begin{flalign}
p &= b^2 - a^2 \\
  &= (b+a)(b-a) \\
  &\implies b+a=p \land b-a=1 \\
  &\implies 2b=p+1 \\
  &\implies b = (p+1)/2 \\
  &\implies a = (p-1)/2 \; ∎\\
\end{flalign}$$

Odd composite integer _n_ = _(2a+1)(2b+1)_ with positive integers _a_ and _b_.  
As can be seen there are at least two differences of squares for n, so not unique.  
So if odd integer _n_ has unique difference of squares, then _n_ is not composite, or prime. ∎

$$\begin{flalign}
n = (2a+1)(2b+1) &= ((a+1)^2-a^2)((b+1)^2-b^2) \\
&= ((a+1)(b+1)+ab)^2 - ((a+1)b+a(b+1))^2\\
&= ((a+1)(b+1)-ab)^2 - ((a+1)b-a(b+1))^2\\
\\
7\times 11 &= (4^2-3^2)(6^2-5^2) & 3\times 7 &= (2^2 - 1^2)(4^2-3^2)\\
          &= 39^2 - 38^2 &         &= 11^2 - 10^2\\
          &= 9^2 - 2^2 &           &= 5^2 - 2^2\\
\end{flalign}$$


Remark: every odd number has representation as canonical difference (1) of squares of a number and its predecessor. Knowing non-canonical reprepresentation (2) for RSA number _n=pq_ with odd primes _p_ and _q_ reveals factorization:  
Just add 2nd square number to first and you get one of the factors _(a+b+1) + (b-a) = 2b+1_, subtract 2nd square number from first and you get the other factor _(a+b+1) - (b-a) = 2a+1_.

$$\begin{flalign}
n = (2a+1)(2b+1) &= ((a+1)^2-a^2)((b+1)^2-b^2) \\
\tag{1}&=(2ab+a+b+1)^2 - (2ab+a+b)^2\\
\tag{2}&=(a+b+1)^2 - (b-a)^2\\
\end{flalign}$$
