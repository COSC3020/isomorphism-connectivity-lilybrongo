# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do *not* have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

Say we have two graphs, $G_1$ and $G_2$. $G_1$ contains vertices A, B, and C. There is an edge between A and B, but there isn't one between A and C, and there isn't onebetween B and C. Graph $G_2$ contains vertices 1, 2, and 3. There is an edge between 1 and 2, but not between 1 and 3 or 2 and 3. We can see that these two graphs have the same overall structure, where some vertices are connected and some vertices are not. Next we can define the mapping. We can create a function f that assigns each vertex in $G_1$ to each vertex in $G_2$. This means $f(A) = 1, f(B) = 2, f(C) = 3$, making sure that every vertex in $G_1$ corresponds to only one vertex in $G_2$. Under this choice of mapping, the edge between A and B in $G_1$ maps to the edge between 1 and 2 in $G_2$. There is no edge between A and C in $G_1$, this matches the missing edge between 1 and 3 in $G_2$. This mapping shows that each connection, or ones not present, do match between the two graphs. Using isomorphic "must-haves", that a one-to-one correspondence (bijection) between their vertices, and that the same conections, or edges, and non-connected edges between corresponding vertices (such as the missing connection bewteen A and C matching to the missing between 1 and 3). Since the mapping of f does satisfy both conditions, $G_1$ and $G_2$ are isomorphic, proving that two graphs do not need to be fully connected to be considered isomorphic. 

Counter example using the given definition:

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

This means that f will map the vertices of $G_1$ to those of $G_2$, maintaining edges and non-edges.

$G_1=(V_1 , E_1)$ with $V_1 =$ {A,B,C} and $E_1 =$ {A,B} 
$G_1$ only consists of 3 vertices where A and B are connected

$G_2=(V_2 , E_2)$ with $V_2 =$ {1,2,3} and $E_2 =$ {1,2} 
$G_2$ consists of only 3 vertices where 1 and 2 are connected

Defining a bijection:
$f: V_1 \rightarrow V_2$
$f(A) = 1, f(B) = 2, f(C) = 3$

Showing the edge-perserving condition:
Edge {A,B} $\in E_1:f(A) = 1, f(B) = 2$ meaning that {1,2} $\in E_2$
Non-Edges(disconnected) {A,C} and {B,C}: $f(A) = 1, f(C) = 3$ so this means that {1,3} $\notin E_2$, which is also the case for {2,3} $\notin E_2$. 

By comparing these isomorphic "must-haves" we can show that $f$ is an isomorphism. Since this also shows that even though $G_1$ and $G_2$ are not fully connected, they are still isomorphic. This proves that two graphs do not need to be completely connected to be isomorphic. 

Referrences:

Geeks for Geeks Graph Isomorphisms and Connectivity: https://www.geeksforgeeks.org/graph-isomorphisms-connectivity/

Identifying Isomorphisms: https://www.youtube.com/watch?v=RoDR40UG--s

Looked at howardtheg8one's repository to get an idea of how to work through this problem. As well as Caden Mcfate who had a drawing in his explination that helped me understand the problem better. 

Also needed to reference github's Writing Mathematical expressions for the layout of my writing
https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions

I certify that I have listed all sources used to complete this exercise, including the use
of any Large Language Models. All of the work is my own, except where stated
otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is
suspected, charges may be filed against me without prior notice.





