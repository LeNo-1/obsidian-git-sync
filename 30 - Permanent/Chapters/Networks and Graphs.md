- **Graph Theory** is a branch of mathematics which is used to model, analyse and solve many real-life problems , and is very useful in problem-solving and mathematical modelling. In Graph Theory a graph has a wider meaning than the usual meaning we take, where we plot a series of points with two perpendicular axes

- DEF: A _graph_ consists of points (known as **vertices**  or __nodes__) which are connected by lines (known as **edges** or __arcs__ )
		Example graph:
<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0" y="0" width="302" height="234" style="
        width:302px;
        height:234px;
        background: #FFF;
        fill: none;
">
        <svg xmlns="http://www.w3.org/2000/svg"/>
        
        <svg xmlns="http://www.w3.org/2000/svg" class="role-diagram-draw-area"><g class="shapes-region" style="stroke: black; fill: none;" ne="0.35232458647546827"><g class="composite-shape"><path class="real" d=" M40,50 C40,45.58 43.58,42 48,42 C52.42,42 56,45.58 56,50 C56,54.42 52.42,58 48,58 C43.58,58 40,54.42 40,50 Z" style="stroke-width: 1; stroke: rgb(0, 0, 0); fill: rgb(230, 153, 162); fill-opacity: 1;" ne="0.07886247684594028"/></g><g class="composite-shape"><path class="real" d=" M42,142 C42,137.58 45.58,134 50,134 C54.42,134 58,137.58 58,142 C58,146.42 54.42,150 50,150 C45.58,150 42,146.42 42,142 Z" style="stroke-width: 1; stroke: rgb(0, 0, 0); fill: rgb(230, 153, 162); fill-opacity: 1;" ne="0.4279058065335022"/></g><g class="composite-shape"><path class="real" d=" M200,217 C200,212.58 203.58,209 208,209 C212.42,209 216,212.58 216,217 C216,221.42 212.42,225 208,225 C203.58,225 200,221.42 200,217 Z" style="stroke-width: 1; stroke: rgb(0, 0, 0); fill: rgb(230, 153, 162); fill-opacity: 1;" ne="0.6723275248376066"/></g><g class="composite-shape"><path class="real" d=" M162,51 C162,46.58 165.58,43 170,43 C174.42,43 178,46.58 178,51 C178,55.42 174.42,59 170,59 C165.58,59 162,55.42 162,51 Z" style="stroke-width: 1; stroke: rgb(0, 0, 0); fill: rgb(230, 153, 162); fill-opacity: 1;" ne="0.821125487168894"/></g><g class="composite-shape"><path class="real" d=" M188,131 C188,126.58 191.58,123 196,123 C200.42,123 204,126.58 204,131 C204,135.42 200.42,139 196,139 C191.58,139 188,135.42 188,131 Z" style="stroke-width: 1; stroke: rgb(0, 0, 0); fill: rgb(230, 153, 162); fill-opacity: 1;" ne="0.9461676777891681"/></g><g class="arrow-line"><path class="connection real" stroke-dasharray="" d="  M48,50 L208,217" style="stroke: rgb(0, 0, 0); stroke-width: 1; fill: none; fill-opacity: 1;" ne="0.5784561704374993"/></g><g class="arrow-line"><path class="connection real" stroke-dasharray="" d="  M50,142 L196,131" style="stroke: rgb(0, 0, 0); stroke-width: 1; fill: rgb(191, 191, 191); fill-opacity: 1;" ne="0.547614309102957"/></g><g class="arrow-line"><path class="connection real" stroke-dasharray="" d="  M48,50 L170,51" style="stroke: rgb(0, 0, 0); stroke-width: 1; fill: none; fill-opacity: 1;" ne="0.7783046923695294"/></g><g class="arrow-line"><path class="connection real" stroke-dasharray="" d="  M50,142 L208,217" style="stroke: rgb(0, 0, 0); stroke-width: 1; fill: none; fill-opacity: 1;" ne="0.3576766574730412"/></g><g class="arrow-line"><path class="connection real" stroke-dasharray="" d="  M48,50 L196,131" style="stroke: rgb(0, 0, 0); stroke-width: 1; fill: none; fill-opacity: 1;" ne="0.4732440079238176"/></g><g/></g><g/><g/><g/></svg>
        <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="300" height="232" style="width:300px;height:232px;font-family:Asana-Math, Asana;background:#FFF;"><g><g><g><text x="44.5" y="22" style="white-space:pre;stroke:none;fill:rgb(191,191,191);fill-opacity:1;font-size:15px;font-family:Arial, Helvetica, sans-serif;font-weight:400;font-style:normal;dominant-baseline:text-before-edge;text-decoration:none solid rgb(191, 191, 191);">A</text></g></g></g><g><g><g><text x="168.5" y="20" style="white-space:pre;stroke:none;fill:rgb(191,191,191);fill-opacity:1;font-size:15px;font-family:Arial, Helvetica, sans-serif;font-weight:400;font-style:normal;dominant-baseline:text-before-edge;text-decoration:none solid rgb(191, 191, 191);">B</text></g></g></g><g><g><g><text x="42.5" y="109" style="white-space:pre;stroke:none;fill:rgb(191,191,191);fill-opacity:1;font-size:15px;font-family:Arial, Helvetica, sans-serif;font-weight:400;font-style:normal;dominant-baseline:text-before-edge;text-decoration:none solid rgb(191, 191, 191);">C</text></g></g></g><g><g><g><text x="195.5" y="101" style="white-space:pre;stroke:none;fill:rgb(191,191,191);fill-opacity:1;font-size:15px;font-family:Arial, Helvetica, sans-serif;font-weight:400;font-style:normal;dominant-baseline:text-before-edge;text-decoration:none solid rgb(191, 191, 191);">D</text></g></g></g><g><g><g><text x="203.5" y="189" style="white-space:pre;stroke:none;fill:rgb(191,191,191);fill-opacity:1;font-size:15px;font-family:Arial, Helvetica, sans-serif;font-weight:400;font-style:normal;dominant-baseline:text-before-edge;text-decoration:none solid rgb(191, 191, 191);">E</text></g></g></g></svg>
</svg>
>*Isomorphic* are graphs that have exactly the **same structure** of vertices and edges, but **labelling may be different** 

- Def. : The *degree* ( or __valency__ or __order__ ) of a a vertex is the number of edges incident to it
- *Handshaking Lemma:* In any graph the **sum of the degrees** will be precisely equal to **2 times the number of edges**

- Def. : A _subgraph_ pf any graph G is any graph, each of whose edges and vertices belong to graph G. It is simply part of the original graph G
- Def. : A _diagraph_ ( or **directed graph** ) is a graph where each of the edges has a **direction associated** with them
- Def. : A *loop* is an edge that **starts and finishes at the same vertex**

- Def. : A graph is a *simple graph* if:
	- It does **not contain any loops**
	- There is no more than **one edge joining any pair of vertices**

- Def. : A graph is *connected* if there is a **path connecting all the vertices** on the graph. A graph is *disconnected* if there are any **vertices on the graph between which there is no path**.
- Def. : A _tree_ is a connected graph with **no cycles**
- Def. : A _spanning tree_ of a graph G is any subgraph of G which includes all the vertices of G and is also a tree
#### Types of routes
- A _walk_ is a route through a graph, from one vertex to another, in which you are permitted to visit each vertex any number of times
	
- A _path_ is a route through a graph, from one vertex to another, in which you are only permitted to visit any vertex once
	
- A _cycle_ is a closed path, where the start and finish vertex of the path are the same, but no other vertex is visited more than once on the path

- Def. : A _tree_ is a connected graph with **no cycles**
- Def. : A _spanning tree_ of a graph G is any subgraph of G which includes all the vertices of G and is also a tree

## Algorithms
### Prim's
- ###### Graph Form
	1. Start at Any Vertex
		- Choose any vertex as the starting point.
		- Select the edge of least weight that is connected to this vertex
	2. Grow the Tree
		- From the set of vertices already included in the tree, choose the edge of least weight that connects to a vertex not yet in the tree.
	    - Ensure that the edge does not create a cycle (i.e., do not connect two vertices already in the tree)[
	
	3. Repeat
		- Continue selecting the lowest-weight edge that connects a vertex in the tree to a vertex outside the tree.
		- Repeat until all vertices are included in the tree
	
	4. Record the Order
		- Keep track of the order in which edges are added to the MST

- ###### Matrix From
	1. Select a Starting Vertex
		- Choose any vertex to start from.
		- Cross out the column for this vertex in the matrix.
		- Label the corresponding row with ‘1’
    
	
	2. Find the Minimum
		- Circle the lowest value in the labelled row (this represents the shortest edge from the current tree).
		- Add this edge to the tree.
		- Cross out the column of the vertex just added.
    
	3. Update Labels
	- Label the row of the newly added vertex with the next number.
	
	4. Repeat
		- Circle the lowest value in any labelled row.
		- Add the corresponding edge to the tree and cross out the relevant column.
		- Continue until all vertices are labelled and included in the tree.

### Dijkstra's
- ###### Graph Form
	
- ###### Matrix Form
	