# cs2040c-assignment-5-sssp-solved
**TO GET THIS SOLUTION VISIT:** [CS2040C Assignment 5-SSSP Solved](https://www.ankitcodinghub.com/product/cs2040c-assignment-5-sssp-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;80785&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS2040C Assignment 5-SSSP  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
In this assignment, we will compute the path and the distance of the shortest path between two nodes. You can assume our graphs are:

<ul>
<li>Directed</li>
<li>At least one node but no limitation on the number of edges.</li>
<li>Each edge has a non-zero positive weight w &gt; 0. Namely, there will be no edge with weight 0 or less</li>
<li>You can assume all computations are in integers.</li>
</ul>
Your graph (together with some SSSP queries) will be given in a text file. You can see there are a few files named “example?.txt” in your folder. Here is an example (example3.txt):

The first line will tell you the number of nodes, edges and SSSP queries. Then followed by e lines of numbers that each line represents an edge with a weight if e is the number of edges. Each edge has three number as the source, the destination and the weight of the edge. After the e lines of edges, it will be followed by q lines of queries. For each query, we will ask “what is the shortest path/distance from one node to another node?”

<h1>Skeleton Code</h1>
You will be given the following code:

<ul>
<li>The Graph Class: ({h,cpp})</li>
<li>The Linked List Skeleton in your Assignment 1 with iterator ({h,cpp})</li>
<li>The driver code (cpp) to read in the input file and start your computations.</li>
</ul>
And you only need to submit the shortest distance function in the file Graph.cpp.

<h1>The Graph Class (Given)</h1>
We use adjacency lists as the data structure for our graphs.&nbsp; For a graph with v nodes, we will have v linked lists and each node a will have a list containing the neighbors of a, together with the weight of the edges. Please see the following diagram as an example:

Each of the Linked List node <u>in the Linked List</u> will be a pair of values of the neighboring node index and the weight of that edge. We create an auxiliary class to help you to store the pair of node number and weight and the class is called NodeWeightPair, in which is just simply a pair of integers.

Please read and understand the functions of the two classes Graph and NodeWeightPair. For example, the member function printGraph() in the Graph class will print out the graph for you:

&nbsp;

<h1>The Linked List Class with Iterators (Given)</h1>
The files simpleLinkedListTemplate.{h,cpp} <strong><em>are</em></strong> the skeleton code of our Assignment 1. However, there are a few additional functions for iterating through a linked list. An example is already in Graph.cpp inside the function printGraph().

for (_al[i].start(); !_al[i].end(); _al[i].next())

cout &lt;&lt; ” (” &lt;&lt; _al[i].current().nodeIndex() &lt;&lt; “,” &lt;&lt; _al[i].current().weight() &lt;&lt; “)”;

<ul>
<li>start() will place a pointer to point to the first item in the Linked List</li>
<li>next() will move the pointer to the next item</li>
<li>end() will return 1 if the current pointer is null, namely, the end of the list, otherwise, return 0.</li>
<li>current() will return the item that the pointer is pointing to currently.</li>
</ul>
&nbsp;

<h1>Task 1 Compute the Shortest Distance for Each Query (50 marks)</h1>
Implement the function shortestDistance(int s, int d) in the class Graph that will return the shortest distance from the node s to the node d. If there is no path from s to d, return -1 instead. For the input file “example3.txt”, your output should be like this:

&nbsp;

In this task, you probably need the priority queue. You can add into your project. But please use the same conventions in the last assignment for the heap. Please bear in mind that you are not allowed to use STL or other code that is not from you.

<h1>Task 2 Printing the Path</h1>
Print the path inside your function shortestDistance() <em>if</em>&nbsp; you can find a path. Your output should be like this for “example4.txt”

&nbsp;

&nbsp;

<h1>Task 3 Problem Solving: Train Trips</h1>
Use your code to solve the following problem by creating an input file without modifying your code in Tasks 1 and 2. There are n cities and you can travel from each city to another by trains. Let’s assume that

<ul>
<li>In every city, the trains are operating 24 hours.</li>
<li>Only some pairs of the cities have trains between them. And luckily, when there is a connection, trains run in both ways, aka, bidirectional. Also, each connection has a different speed limit for the trains</li>
<li>Every train will leave a city at <em>every</em> Namely, there will be a train leaving at 12:00, 1:00, 2:00, 3:00, and so on.</li>
<li>You are provided with the information of how long the distance is between two cities, and the speed limit of the trains between the two cities, see the table below.</li>
<li>You can assume every train will gain its speed to its maximum speed, and brake, in no time.</li>
<li>And you can also transfer from train to train in no time.</li>
</ul>
Here is the distance and maximum speed for the trains between 8 cities. The <strong>first number</strong> in each cell is the distance between the two places in km. The second number is the speed limit in km per hour. Note that the matrix is symmetric and we omit the other half. Namely, the entry with Cities 0 to 1 and 1 to 0 should be the same as (200,40).

<table width="672">
<tbody>
<tr>
<td colspan="9" width="672"><strong>Cities &nbsp;&nbsp;&nbsp; 0 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 6 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 7 </strong></td>
</tr>
<tr>
<td width="74"><strong>0 </strong></td>
<td width="75"></td>
<td width="74">200,40</td>
<td width="75"></td>
<td width="74">150,30</td>
<td width="75">100,25</td>
<td width="76"></td>
<td width="74"></td>
<td width="74"></td>
</tr>
<tr>
<td width="74"><strong>1 </strong></td>
<td width="75"></td>
<td width="74"></td>
<td width="75">80,40</td>
<td width="74"></td>
<td width="75"></td>
<td width="76">200,100</td>
<td width="74"></td>
<td width="74"></td>
</tr>
<tr>
<td width="74"><strong>2 </strong></td>
<td width="75"></td>
<td width="74"></td>
<td width="75"></td>
<td width="74"></td>
<td width="75">160,40</td>
<td width="76">90,45</td>
<td width="74">240,60</td>
<td width="74"></td>
</tr>
<tr>
<td width="74"><strong>3 </strong></td>
<td width="75"></td>
<td width="74"></td>
<td width="75"></td>
<td width="74"></td>
<td width="75"></td>
<td width="76"></td>
<td width="74"></td>
<td width="74"></td>
</tr>
<tr>
<td width="74"><strong>4 </strong></td>
<td width="75"></td>
<td width="74"></td>
<td width="75"></td>
<td width="74"></td>
<td width="75"></td>
<td width="76"></td>
<td width="74">300,60</td>
<td width="74"></td>
</tr>
<tr>
<td width="74"><strong>5 </strong></td>
<td width="75"></td>
<td width="74"></td>
<td width="75"></td>
<td width="74"></td>
<td width="75"></td>
<td width="76"></td>
<td width="74">300,30</td>
<td width="74">360,60</td>
</tr>
<tr>
<td width="74"><strong>6 </strong></td>
<td width="75"></td>
<td width="74"></td>
<td width="75"></td>
<td width="74"></td>
<td width="75"></td>
<td width="76"></td>
<td width="74"></td>
<td width="74">270,30</td>
</tr>
<tr>
<td width="74"><strong>7 </strong></td>
<td width="75"></td>
<td width="74"></td>
<td width="75"></td>
<td width="74"></td>
<td width="75"></td>
<td width="76"></td>
<td width="74"></td>
<td width="74"></td>
</tr>
</tbody>
</table>
Create an input file that can use your code to answer the following question: <strong>What is the shortest time (in hours) and the path to go from City 0 to City 7</strong>?
