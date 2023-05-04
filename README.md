Download Link: https://assignmentchef.com/product/solved-csci-3104-assignment-5
<br>
<ol>

 <li>Write a dynamic programming algorithm to solve the longest increasing subsequence (LIS) problem. You are given an array <em>A </em>of <em>n </em> An <em>increasing subsequence </em>is a sequence of <em>k </em>indices 0 ≤ <em>i</em><sub>1 </sub><em>&lt; i</em><sub>2 </sub><em>&lt; … &lt; i<sub>k </sub></em>≤ (<em>n </em>− 1) such that <em>A</em>[<em>i</em><sub>1</sub>] <em>&lt; A</em>[<em>i</em><sub>2</sub>] <em>&lt; … &lt; A</em>[<em>i<sub>k</sub></em>]. Thus, given an array <em>A</em>, you are to compute an increasing subsequence <em>i</em><sub>1</sub><em>,…,i<sub>k </sub></em>whose length <em>k </em>is the longest possible.</li>

</ol>

Example: <em>A </em>= [1<em>,</em>5<em>,</em>2<em>,</em>3<em>,</em>8]. The longest increasing subsequence has length 4 with corresponding indices <em>i </em>= [0<em>,</em>2<em>,</em>3<em>,</em>4].

Let’s define the function LIS(A, j, M) to be length of the LIS for the first <em>j </em>elements of the array (<em>A</em>[0]<em>,…,A</em>[<em>j </em>− 1]), where <em>j </em>ranges from 0 to <em>n </em>and all elements of this subsequence are less than <em>M</em>.

<ol>

 <li>For <em>A </em>= [1<em>,</em>5<em>,</em>2<em>,</em>3<em>,</em>8], write down the values of LIS(A, 4, 3) and LIS(A, 5, ∞).</li>

 <li>Write down the base case for LIS(A, 0, M).</li>

 <li>Write down the recurrence for LIS(A, j, M) for any 1 ≤ <em>j </em>≤ <em>n</em>.</li>

 <li>Describe a scheme to memoize the recurrence LIS</li>

 <li>Implement your dynamic programming algorithm scheme in Python. Input to your function is the array <em>A</em>, and the output should be the LIS itself.</li>

</ol>

<ol start="2">

 <li>One of Gru’s favorite games to watch is a game played by his minions. The game works as follows: The game is played on an <em>n </em>x <em>n </em>square grid by a minion. The minion starts by placing a token on any square of the grid. On each turn, the minion moves the token either one square down, or one square to the right. The game finishes when the token is moved off the edge of the board. Each square on the grid has some numerical value (could be positive, negative, or zero). The initial score for the minion is zero, and each time the token lands on a square, its value gets added to the minion’s score. The goal of the game is to score as many points as possible.

  <ol>

   <li>Provide an algorithm (pseudocode) to compute the maximum possible score for this game, given an <em>n </em>x <em>n </em>array of values as input.</li>

   <li>Prove the correctness of your algorithm.</li>

   <li>Analyze your algorithm’s time and space complexities.</li>

  </ol></li>

 <li>Gru claims he can determine whether a directed graph <em>G</em>, when represented by an adjacency matrix, contains a black hole in O(<em>V </em>) time. A black hole is defined as a vertex with in-degree |<em>V </em>|−1 (every other vertex points to this one) and out-degree 0. Prove that Gru is correct, and provide pseudocode for this algorithm (the algorithm to determine whether a graph <em>G </em>contains a black hole, given that <em>G </em>is represented as an adjacency matrix).</li>

</ol>

1

<ol start="4">

 <li>a) Gru, always curious, gives you an array <em>A </em>of numbers, with length <em>n</em>, and he aims to find an algorithm to find out if any two elements of the array <em>A </em>sum to <em>T</em>. For example, suppose <em>A </em>= [14<em>,</em>−36<em>,</em>21<em>,</em>4<em>,</em>9<em>,</em>41]. If <em>T </em>= 25, the result is TRUE because <em>A</em>[2] + <em>A</em>[3] = 25. However, if <em>T </em>= −1, the result would be FALSE, since no two elements in <em>A </em>sum to −1.</li>

</ol>

Of course, Gru assigns <em>you </em>the task of writing a Python function sumTwo(A, T) that determines if, for the given array <em>A</em>, two elements sum to <em>T</em>. Since Gru is always interested in efficiency, he informs you that your algorithm must run in Θ(<em>n</em>) in the average case (<strong>Hint: </strong>Use a hashtable).

<ol>

 <li>b) Now Gru asks you to write a Python function sumThree(A, T) which checks if three elements in <em>A </em>sum to <em>T </em>(<strong>Hint: </strong>Use your function from part (a) as a subroutine).</li>

</ol>


