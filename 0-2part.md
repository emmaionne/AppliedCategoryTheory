
**What is a conceptual Graph?**

**Definition 1** (Conceptual Graph). A conceptual graph $G$ consist of $G=(P(G), V(G); \partial_G:P(G) \rightarrow V(G)\times V(G), \iota_G: V(G) \hookrightarrow P(G) )$ where 
- $P(G)$ is the set of parts of $G$,
- $V(G)$ is the set of vertices of the graph $G$,
- $V(G) \times V(G)$ is the set of unordered pairs of vertices of $G$,
- $\partial_G$ is the incidence map and $\iota_G$ is the inclusion map of the vertex set into the part set.

The set of parts is created by joining the set of vertices and the set of edges. So the set of edges $E(G)$ can be defined by $E(G) = P(G) / \iota_G(V(G))$. The set of unordered pairs of vertices of $G$ is the set of all posible pair of vertices in a graph $G$, where the order of the vertices in each pair does not matter. So this paper works with undirected graphs. We can already consider the question of whether the definition of conceptual graphs can be broadened to include directed graphs? 

**Definition 2** (Graph Homomorphism). $f:G \rightarrow H$ is a graph (homo)morphism of conceptual graphs from $G$ to $H$ if $f$ is a function 
- $f_P:P(G) \rightarrow P(H)$ and
- $f_V:V(G) \rightarrow V(H)$ that preserves incidence, that is to say,

$\partial_H(f_P(e))=f_V(x) \sim f_V(y)$ whenever $\partial_G(e) = x \sim y$ for all $e \in P(G)$, $x,y \in V(G)$.

