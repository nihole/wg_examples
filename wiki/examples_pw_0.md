**++0++**

This is a root node with the statement under discussion!

Each graph node has 4 attributes:
- **id**: any text identifying the node (I usually use the --n-- or ++n++ format, but this is not required. But in any case, the id must be unique.)
- brief **description** that presents this node on the graph 
- **link** to the article with detailed explanation of this statement
- downward directed (or bidirectional in case of complement) graph **edges** 

Graph edges represent the relation between nodes. We have only 2 types of such relations:
- **refutation** (rebuttal, contradiction)
- **complement** (logical 'not')

All other relationships are expressed via these 2 types. This is very similar to boolean logic where everything may be expressed via pare of and/not or or/not.

It is possible to introduce a metric for the relation strength, but this is usually quite subjective and we will only use 2 levels, which leads to the fact that refutation may have 2 types of strength:
- direct refutation (rebuttal, contradiction)
- indirect refutation (rebuttal, contradiction)

So as result цe have 4 types of dependence of A on B:
- **Independence** (A does not depend on B). The truth or falsity of statement A does not depend in any way on the truth or falsity of statement B.

- **Direct rebuttal**. If statement B is true, then statement A is false. We will denote such a relationship as **A --d-> B**. This arrow **--d->** actually can be replaced with expression "false because", that is, A --p-> B is a short expression of the expression "A false because B (is true) ". 
On the graph, we will denote this connection by a solid line with an arrow from A to B.

- **Indirect refutation**. If statement B is true, then the probability that statement A is false increases. We will call this an indirect refutation and denote it as **A --i-> B**. On the graph, we will denote it by a dotted line with an arrow from A to B.

- **Complement** (logical negation). If statement B is true, then statement A is false, and if statement B is false, then statement A is true. We will denote this as **A <-> B**. It is easy to show that if A <-> B, then B <-> A. On the graph, this connection will be denoted by a solid line with a double-headed arrow.
