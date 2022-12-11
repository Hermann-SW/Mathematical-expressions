# Mathematical-expressions

# example from doc

From:  
https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions  
This sentence uses `$` delimiters to show math inline:  $\sqrt{3x-1}+(1+x)^2$

Works even when edited on github with Preview ...

## From my Obsidian "Number theory" vault
[Odd prime iff unique difference of 2 squares.md](Number%20theory/Odd%20prime%20iff%20unique%20difference%20of%202%20squares.md)

## 1st problem 
This is a formula with factorial, powers of 2 and odd numbers I tweeted on the weekend:  
$(2^n)! \cdot 2 = 2^{2^n} \cdot  \prod_{j=1}^{n-1} \enspace  \prod_{i=2^{n-j-1}+1}^{2^{n-j}}(2i-1)^{j}$

My fault that above formula looked that bad, I used single '$' for inline formula.  
Framing with '$$' the products look much better now:  
$$(2^n)! \cdot 2 = 2^{2^n} \cdot  \prod_{j=1}^{n-1} \enspace  \prod_{i=2^{n-j-1}+1}^{2^{n-j}}(2i-1)^{j}$$

Similar to screenshot from Latex rendered formula:  
<kbd>
![factorial_pow2_odd.png](factorial_pow2_odd.png)
</kbd>

## multiline eqnarray* works as well

$$\begin{eqnarray*}
& & &     (2n)!    & = & n! 2^n \prod_{i=1}^{n}(2i-1) & & (1)\\
& & &     (2^n)!   & = & (2^{n-1})! 2^{2^{n-1}} \prod_{i=1}^{2^{n-1}}(2i-1) & & (2)\\
& & &              & = & (2^{n-2})! 2^{2^{n-2}} 2^{2^{n-1}} \prod_{i=1}^{2^{n-2}}(2i-1)  \prod_{i=1}^{2^{n-1}}(2i-1)\\
& & &              & = & (2^{n-3})! 2^{2^{n-3}} 2^{2^{n-2}} 2^{2^{n-1}} \prod_{i=1}^{2^{n-3}}(2i-1) \prod_{i=1}^{2^{n-2}}(2i-1)  \prod_{i=1}^{2^{n-1}}(2i-1)\\
& & &              & = & 2^{2^0} \cdot \dots \cdot 2^{2^{n-3}} \cdot 2^{2^{n-2}} \cdot 2^{2^{n-1}} \cdot \prod_{i=1}^{2^1}(2i-1) \cdot \dots \cdot \prod_{i=1}^{2^{n-3}}(2i-1) \cdot \prod_{i=1}^{2^{n-2}}(2i-1)  \prod_{i=1}^{2^{n-1}}(2i-1)  & & (3)\\
& & &              & = & 2^{2^n-1} \cdot \prod_{i=1}^{2^1}(2i-1) \cdot \dots \cdot \prod_{i=1}^{2^{n-3}}(2i-1) \cdot \prod_{i=1}^{2^{n-2}}(2i-1)  \prod_{i=1}^{2^{n-1}}(2i-1)\\
& & &              & = & 2^{2^n-1} \prod_{j=1}^{n-1} \enspace  \prod_{i=2^{n-j-1}+1}^{2^{n-j}}(2i-1)^{j} \\
& & &     (2^n)! \cdot 2  & =& 2^{2^n} \cdot  \prod_{j=1}^{n-1} \enspace  \prod_{i=2^{n-j-1}+1}^{2^{n-j}}(2i-1)^{j} \\
\textrm{Alternatively from (3):}& \\ 
& & &      (2^n)!   & = & 2^{2^n-1} \cdot \prod_{j=1}^{n-1} \enspace  \prod_{i=1}^{2^{n-j}}(2i-1) 
\end{eqnarray*}$$

