# PathFinding-Vistualization

<h3>Modules:</h3>
    <ul>
        <li> pygame
        <li>math
        <li>Priority Queue
    </ul>

<h3>Algorithm:</h3>   
A* is a variant of Dijkstra's algorithm commonly used in games. A* assigns a weight to each open node equal to the weight of the edge to that node plus the approximate distance between that node and the finish. This approximate distance is found by the heuristic, and represents a minimum possible distance between that node and the end. This allows it to eliminate longer paths once an initial path is found. If there is a path of length x between the start and finish, and the minimum distance between a node and the finish is greater than x, that node need not be examined.  <br><br>
    f(x) = h(x) = g(x)<br>
    h(x) = heuristic estimate function<br> 
    g(x) = distance from start node and end node<br><br>
  A* uses this heuristic to improve on the behavior relative to Dijkstra's algorithm. When the heuristic evaluates to zero, A* is equivalent to Dijkstra's algorithm. As the heuristic estimate increases and gets closer to the true distance, A* continues to find optimal paths, but runs faster (by virtue of examining fewer nodes). When the value of the heuristic is exactly the true distance, A* examines the fewest nodes. (However, it is generally impractical to write a heuristic function that always computes the true distance, as the same comparison result can often be reached using simpler calculations – for example, using Manhattan distance over Euclidean distance in two-dimensional space.) As the value of the heuristic increases, A* examines fewer nodes but no longer guarantees an optimal path. In many applications (such as video games) this is acceptable and even desirable, in order to keep the algorithm running quickly.
