---
layout: default
title: What is Markov Chain? 
---

# What is Markov Chain? 6

A Markov Chain, also called Markov Process, is a stochastic (that is random) process, where the probability of the process transitioning to any state depends solely on the current state of the process. For the sake of simplicity, this discussion will be limited to discrete-time Markov Chains.

### Formal Definition
Let $X_n, n=0,1,2,...$ be a  stochastic process that takes a countable number of possible values. Let these possible values be indexed by the set of integers \\(\left \\{ 1,2,3,... \right \\}\\). If $X_{n}=i$, the process is said to be in state \\(i\\) at time \\(n\\). When the process is in state \\(i\\), let there be a fixed probability \\(P_{ij}\\) that it will next be in state \\(j\\). Such a stochastic process is called a Markov Chain.

Because probabilities are always non-negative and the process must make a transition at every increment in $t$ from current state $i$ in to some state $j$ (note, $j$ may or may not be equal to $i$), we have

<div align="center">
$$ P_{ij} \geq 0, \hspace{1em} i,j \geq 0, \hspace{1em} \sum_{j=0}^\infty P_{ij} = 1 $$
</div>

### What does it mean in plain English?
A Markov Chain is a stochastic process such that:
- At any given time, the process is in some state.
- All the states that the process can assume are known.
- The total number of states that the process can assume is either a finite number or countably infinite.
- At every unit increment in time, the process transitions from its current state to some state. The new state may or may not be the same as the current state.
- For every possible state $i$, the probability of transitioning to every possible state is fixed and defined; and adds up to \\(1\\).
- That's it.


### One-step transition probability matrix
As mentioned above, for every possible state $i$, the probability of transitioning to every possible state is fixed and defined. These probability values can be put in to a matrix form for ease of mathematical manipulation, and this matrix is called one-step transition probability matrix &mdash; because, it is the probability matrix for a single time-step. It fully defines the given Markov process. The matrix is defined as follows:

<div align="center">
$$ \begin{pmatrix}
 &P_{00}  &P_{01}  &P_{02}  &... \\
 &P_{10}  &P_{11}  &P_{12}  &... \\
 &\vdots  &\vdots  &\vdots \\
 &P_{i0}  &P_{i1}  &P_{i2}  &... \\
 &\vdots  &\vdots  &\vdots \\
\end{pmatrix}
$$
</div>
