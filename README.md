<h1>ExpNo 3 : Implement Breadth First Search Traversal of a Graph</h1> 
<h3>Name: THANJIYAPPAN K</h3>
<h3>Register Number: 212222240108</h3>
<H3>Aim:</H3>
<p>To Implement Breadth First Search Traversal of a Graph using Python 3.</p>
<h3>Theory:</h3>
<p>Breadth-First Traversal (or Search) for a graph is like the Breadth-First Traversal of a tree.
The only catch here is that, unlike trees, graphs may contain cycles so that we may come to the same node again. To avoid processing a node more than once, we divide the vertices into two categories:
<ol><li>Visited</li>
<li>Not Visited</li></ol>
</p>
<p>A Boolean visited array is used to mark the visited vertices. For simplicity, it is assumed that all vertices are reachable from the starting vertex. BFS uses a queue data structure for traversal.</p>
<p><strong>How does BFS work?</strong><br>
  Starting from the root, all the nodes at a particular level are visited first, and then the next level nodes are traversed until all the nodes are visited.
To do this, a queue is used. All the adjacent unvisited nodes of the current level are pushed into the queue, and the current-level nodes are marked visited and popped from the queue.
Illustration:
Let us understand the working of the algorithm with the help of the following example.
Step1: Initially queue and visited arrays are empty.
</p>

![image](https://github.com/natsaravanan/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/87870499/8acdebf8-ecc2-4d10-a208-45cce441f059)


Queue and visited arrays are empty initially.
Step2: Push node 0 into queue and mark it visited.

![image](https://github.com/natsaravanan/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/87870499/0e9ce012-8e1f-43d7-b7b9-c0fb19fe0c3f)


Push node 0 into queue and mark it visited.
Step 3: Remove node 0 from the front of queue and visit the unvisited neighbours and push them into queue.

![image](https://github.com/natsaravanan/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/87870499/67d8fa3b-ce9e-46c2-9dd7-089e204e667a)

Step 4: Remove node 1 from the front of queue and visit the unvisited neighbours and push them into queue.

![image](https://github.com/natsaravanan/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/87870499/b0cf0fde-8a86-41cb-a054-36875ac24ab0)

Step 5: Remove node 2 from the front of queue and visit the unvisited neighbours and push them into queue.

![image](https://github.com/natsaravanan/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/87870499/8968a163-6b3a-4f7e-8ad4-bbf24f326b9b)

Step 6: Remove node 3 from the front of queue and visit the unvisited neighbours and push them into queue. 
As we can see that every neighbours of node 3 is visited, so move to the next node that are in the front of the queue.

![image](https://github.com/natsaravanan/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/87870499/7a1c1b16-ea69-497f-a099-8440200f6dc0)

Steps 7: Remove node 4 from the front of queue and visit the unvisited neighbours and push them into queue. 
As we can see that every neighbours of node 4 are visited, so move to the next node that is in the front of the queue.

![image](https://github.com/natsaravanan/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/87870499/8e16ffa3-c3d6-4774-822b-6eb84adedad9)

Remove node 4 from the front of queue and visit the unvisited neighbours and push them into queue.
Now, Queue becomes empty, So, terminate these process of iteration.


<hr>
<h2>Algorithm:</h2>
<hr>
<ol>
  <li>Construct a Graph with Nodes and Edges</li>
 <li>Breadth First Uses Queue and iterates through the Queue for Traversal.</li>
  <li>Insert a Start Node into the Queue.</li>
<li>Find its Successors Or neighbors and Check whether the node is visited or not.</li>
<li>If Not Visited, add it to the Queue. Else Continue.</li>
<li>Iterate steps 4 and 5 until all nodes get visited, and there are no more unvisited nodes.</li>

</ol>

## Program:
```
def percept(self, agent):
    return agent.location, self.status[agent.location]
def execute_action(self, agent, action): 
    if action == "Right":
        agent.location = room_B
        agent.performance -= 1
    elif action == "Left":
        agent.location = room_A
        agent.performance -= 1
    elif action == "suck":
        self.status [agent.location] == "dirty"
        agent.performance += 10
    self.status[agent.location] = "clean"
    
    
    
    
    
    
    
def SimpleHillClimbing(answer):
    best-generate_random_solution(answer)
    best_score=evaluate(best,answer)
    while True:
        if best_score==0:
            print("Score:",best_score," Solution : ","".join(best))
            break
        new_solution=mutate_solution(list(best))
        score=evaluate(new_solution, answer)
        if score<best_score:
            best=new_solution
            best_score=score    
            
            
            
            
            
            
            
            
            
from itertools import permutations
def solvecrypt():
    for perm in permutations (range(10),8):
        S,E,N,D,M,O,R,Y=perm
        if S==0 or M==0:
            continue
        SEND=S*1000+E*100+N*10+D
        MORE= M*1000+O*100+R*10+E
        MONEY=M*10000+O*1000+N*100+E*10+Y
        if SEND+ MORE==MONEY:
            print("SEND",SEND)
            print("MORE ",MORE)
            print("MONEY",MONEY)
solvecrypt()            
    
    
    
from itertools import permutations    
def solvecrypt():
    for perm in permutations (range(10),9):
        C,R,O,S,A,D,N,G,E=perm
        if C==0 or R==0:
            continue
        CROSS=C*10000+R*1000+O*100+S*10+S
        ROADS=R*10000+O*1000+A*100+D*10+S
        DANGER=D*100000+A*10000+N*1000+G*100+E*10+R
        if CROSS+ ROADS==DANGER: 
            print("CROSS", CROSS) 
            print("ROADS", ROADS)
            print ("DANGER", DANGER)
solvecrypt()    
    
    
    
    
    
from itertools import permutations
def solvecrypt():
    for perm in permutations (range(10),6):
        E,A,T,H,P,L=perm
        if E==0 or T==0:
             continue
        EAT= E*100+A*10+T
        THAT=T*1000+H*100+A*10+T
        APPLE=A*10000+P*1000+P*100+L*10+E
        if EAT + THAT==APPLE:
            print("EAT", EAT) 
            print("THAT", THAT)
            print ("APPLE", APPLE)
solvecrypt()    
    
    
    
    
    
    
    
def dfs(graph,start,visited,path):
   path.append(start)
   visited[start]=True
   for neighbour in graph[start]:
       if visited[neighbour]==False:
           dfs(graph,neighbour,visited,path)
           visited[neighbour]=True
   return path
   
   
   
   
   
   
   
   
def bfs(graph,start,visited,path):
    queue = deque()
    path.append(start)
    queue.append(start)
    visited[start] = True
    while len(queue) != 0:
        tmpnode = queue.popleft()
        for neighbour in graph[tmpnode]:
            if visited[neighbour] == False:
                path.append(neighbour)
                queue.append(neighbour)
                visited[neighbour] = True
                return path   
    
    
    
    
    
```
<hr>
<h3>Sample Input</h3>
<hr>
7 9 <BR>
A B <BR>
A C <BR>
A F <BR>
C E <BR>
C F <BR>
C D <BR>
D E <BR>
D G <BR>
G F <BR>
<hr>
<h3>Sample Output</h3>
<hr>
['A', 'B', 'C', 'F', 'E', 'D', 'G']

<hr>

<hr>
<h3>Sample Input</h3>
<hr>
5 6 <BR>
0 1 <BR>
0 2 <BR>
1 2 <BR>
1 3 <BR>
2 4 <BR>
3 4 <BR>
<hr>
<h3>Sample Output</h3>
<hr>
['0', '1', '2', '3', '4']
<hr>
<h3>Result:</h3>
<hr>
<p>Thus,a Graph was constructed and implementation of Breadth First Search for the same graph was done successfully.</p>
