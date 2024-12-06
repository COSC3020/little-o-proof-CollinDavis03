# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

## Defintions

**Big O Definition** 
$f(n) \in O(g(n)) \iff \exists c > 0, \exists n_{0} > 0$ such that $f(n) \leq c * g(n), \forall n \geq n_{0}$

**Little O Definition**
$f(n) \in o(g(n)) \iff \forall c > 0, \exists n_{0} > 0$ such that $f(n) < c * g(n), \forall n \geq n_{0}$

## Proof
From the definition of little o, we know that any constant c > 0, there exists $n_{0} > 0$ such that: 

$f(n) < c * g(n), \forall n \geq n_{0}$

in particular, we can choose some constant c > 0, and the above condition holds. Since $f(n) < c * g(n) \Rightarrow f(n) \leq c * g(n)$, this satisfies the condition for $f(n) \in O(g(n)), where at least one c > 0 works. 

Thus by definition of Big O, we conclude 

$f(n) \in O(g(n))$

## Sources
The only source I used was JamesOzzyBurn's repo to make sure I did it right, which I did. The only thing I missed was spelling the right arrow markdown part wrong. Other than that, I just used the resources provided in class to solve this and checked Jame's repo to make sure I did it right. 

## Plagarism Statement
“I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.”
