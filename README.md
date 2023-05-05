Download Link: https://assignmentchef.com/product/solved-data-structures-and-algorithms-cs-f211-sheet-11
<br>
<strong> </strong><span style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">Each time Sunny and Johnny take a trip to the Ice Cream Parlour, they pool their money to buy ice cream. On any given day, the parlour offers a line of flavours. Each flavour has a cost associated with it. Given the value of money and the cost of each flavour for trips to the Ice Cream Parlour, help Sunny and Johnny choose two distinct flavours such that they spend their entire pool of money during each visit. ID numbers of the ice creams are </span><em style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">1- based</em><span style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;"> index numbers associated with a cost. For each trip to the parlour, print the ID numbers for the two types of ice cream that Sunny and Johnny purchase as two space-separated integers on a new line. You must print the smaller ID first and the larger ID second.</span>




<strong>Input: </strong>

The first 3 input lines are as follows:

The first line contains total amount money.

The second line contains an integer, <strong><em>n</em></strong>, the size of the array cost.

The third line contains <strong><em>n</em></strong> space-separated integers denoting the <strong><em>cost[i]</em></strong>.




<strong>Output: </strong>

Print two space-separated integers denoting the respective indices for the two distinct flavours they choose to purchase in ascending order. Note that multiple answers may be possible. In that case, print only one answer.




<strong>Sample Input: </strong>

7

6

1 5 4 6 9 7

<strong> </strong>

<strong>Sample Output: </strong>

1 6




<ol start="2">

 <li>Harold is a kidnapper who wrote a ransom note, but now he is worried it will be traced back to him through his handwriting. He found a magazine and wants to know if he can cut out whole words from it and use them to create an untraceable replica of his ransom note. The words in his note are <em>case-sensitive</em> and he <em>must</em> use only whole words available in the magazine. He <em>cannot </em>use substrings or concatenation to create the words he needs.</li>

</ol>

Given the words in the magazine and the words in the ransom note, print Yes if he can replicate his ransom note <em>exactly</em> using whole words from the magazine; otherwise, print No.

For example, the note is “Attack at dawn”. The magazine contains only “attack at dawn”. The magazine has all the right words, but there’s a case mismatch. The answer is No.




<strong>Input: </strong>

The first line contains two space-separated integers, <strong><em>m</em></strong> and <strong><em>n</em></strong>, the numbers of words in the magazine and the note.

The second line contains <strong><em>m</em></strong> space-separated strings, each is <strong><em>magazine[i]</em></strong>.  The third line contains <strong><em>n</em></strong> space-separated strings, each <strong><em>note[i]</em></strong>.

<strong> </strong>

<strong>Output:</strong>

Print Yes if he can use the magazine to create an untraceable replica of his ransom note. Otherwise, print No.

<strong> </strong>

<strong> </strong>

<strong>Example: </strong>

6 4

give me one grand today night give one grand today

<strong> </strong>

<strong>Answer: </strong>

Yes




<ol start="3">

 <li>Given a Binary Tree, write a function that returns the size of the largest subtree which is also a Binary Search Tree in terms of the number of nodes present in it. If the complete Binary Tree is BST, then return the size of the whole tree.</li>

</ol>




<strong>Input: </strong>

First line contains number of nodes, <strong><em>n</em></strong>.

The next <strong><em>n-1</em></strong> lines contain value of nodes which are connected. Last line contains root.

<strong> </strong>

<strong>Output: </strong>

Size of the maximum subtree which is BST.

All the nodes which are in the subtree.

<strong> </strong>

<strong>Example: </strong>

5

<h1>5 2</h1>

5 4

2 1

<ul>

 <li>3</li>

</ul>

5

<strong> </strong>

<strong>Answer: </strong>

<ul>

 <li>2 1 3</li>

</ul>




<ol start="4">

 <li>Shantam is very rich. He is extremely talented in almost everything except in mathematics. So, one day, he pays a visit to a temple (to pray for his upcoming mathematics exams) and decides to donate some amount of money to the poor people (everyone is poor on a relative scale to Shantam). He orders <strong><em>N</em></strong> people to sit in a linear arrangement and indexes them from <strong><em>1 </em></strong>to<strong><em> N</em></strong>, to ease the process of donating money. As with all rich people, their way of doing things is completely different. Shantam donates his money in <strong><em>M</em></strong> steps, each of his step being to choose two indices <strong><em>L</em></strong> and <strong><em>R</em></strong>, and an amount of money <strong><em>C</em></strong> and then he donates <strong><em>C</em></strong> currencies to each and every person whose index lies in <strong><em>[L, R]</em></strong>. In other words, he donates <strong><em>C</em></strong> currencies to every index <strong><em>i</em></strong> such <strong><em>L &lt;= i &lt;= R</em></strong>.</li>

</ol>




Luckily, you too were among the <strong><em>N</em></strong> people selected and somehow you know all the <strong><em>M</em></strong> steps in advance. Figure out the maximum amount of money you can obtain and at what position you should sit to get this maximum amount of money. If multiple positions guarantee the maximum amount of money, output the minimum index out of all these possibilities.




You will be given initial <strong><em>L[1], R[1] and C[1]</em></strong> (which points to step 1) as well as <strong><em>P , Q </em></strong>and<strong><em> S</em></strong> (integer numbers to calculate <strong><em>L, R </em></strong>and<strong><em> C</em></strong> for steps <strong><em>i &gt; 1</em></strong>). Each subsequent step (<strong><em>i &gt; 1</em></strong>) is generated as:




L[i] = (L[i-1] * P + R[i-1]) % N + 1;

R[i] = (R[i-1] * Q + L[i-1]) % N + 1;

if(L[i] &gt; R[i]) swap(L[i] , R[i]);

C[i] = (C[i-1] * S) % 1000000 + 1;




<strong>Input: </strong>

The first line contains <strong><em>T</em></strong>, the number of test cases. The first line of each test case contains two space separated integers <strong><em>N</em></strong> and <strong><em>M</em></strong>, which denotes the number of people and the number of steps, respectively. The next line contains integers <strong><em>L, R, C , P , Q </em></strong>and<strong><em> S </em></strong>, which are used to generate the queries using the method specified above.

<strong> </strong>

<strong>Output: </strong>

For each test case, output one line containing two space separated integers, the first being the optimal position and the second being the highest amount of money that can be obtained.

<strong> </strong>

<strong>Example: </strong>

<h1>2</h1>

5 2

1 1 1 1 1 1

<h1>5 1</h1>

1 3 2 4 3 5

<strong> </strong>

<strong>Answer: </strong>

3 2

1 2




<ol start="5">

 <li>Given a Binary Search Tree (BST) and a range <strong><em>[min, max]</em></strong>, remove all keys which are outside the given range. The modified tree should also be BST.</li>

</ol>

<strong> </strong>

<strong>Input- </strong>

First line contains number of nodes, <strong><em>n</em></strong>.

The next <strong><em>n-1</em></strong> lines contain value of nodes which are connected.

The next line contains root.

The last line contains the range <strong><em>[min, max]</em></strong>.

<strong> </strong>

<strong>Output- </strong>

Output the in-order traversal of the final binary search tree.




<strong>Example: </strong>

7

6 -13

6 14

-13 -8

14 13

14 15

13 7

6

-10 13

<strong> </strong>

<strong>Answer: </strong>

6 -8 13 7




<ol start="6">

 <li>You are the owner of a library. Now you need to setup a search engine for all the books in the library. Your search engine should also be able to auto correct few mistakes done by user.</li>

</ol>

Given a list of book names, we want to implement a spellchecker that converts a query word into a correct word. For a given query word, the spell checker handles two categories of spelling mistakes:




<strong>Capitalization:</strong> If the query matches a word in the book names (case-insensitive), then the query word is returned with the same case as the case in the wordlist.

<ul>

 <li>Example: books= [“yellow”], query = “YellOw”: correct = “yellow”</li>

 <li>Example: books= [“Yellow”], query = “yellow”: correct = “Yellow”</li>

 <li>Example: books= [“yellow”], query = “yellow”: correct = “yellow”</li>

</ul>




<strong>Vowel Errors:</strong> If after replacing the vowels (‘a’, ‘e’, ‘i’, ‘o’, ‘u’) of the query word with any vowel individually, it matches a word in the wordlist (case-insensitive), then the query word is returned with the same case as the match in the wordlist.

<ul>

 <li>Example: books= [“YellOw”], query = “yollow”: correct = “YellOw”</li>

 <li>Example: books= [“YellOw”], query = “yeellow”: correct = “” (no match)</li>

 <li>Example: books= [“YellOw”], query = “yllw”: correct = “” (no match)</li>

</ul>




In addition, the spell checker operates under the following precedence rules:

<ul>

 <li>When the query exactly matches a word in the wordlist (case-sensitive), you should return the same word back.</li>

 <li>When the query matches a word up to some capitalization errors, you should return the first such match in the wordlist.</li>

 <li>When the query matches a word up to some vowel errors, you should return the first such match in the wordlist.</li>

 <li>If the query has no matches in the wordlist, you should return the empty string.</li>

</ul>




Given some queries, return a list of words answer, where <strong><em>answer[i]</em></strong> is the correct word for <strong><em>query = queries[i]. </em></strong>




<strong>Sample Input Format: </strong>

<strong><em>N </em></strong>– number of books

<strong><em>N</em></strong> lines contain the name of books

<strong><em>Q</em></strong> – number of queries

<strong><em>Q</em></strong> lines for each query word




<strong>Sample Input: </strong>

4 KiTe kite hare Hare 10 kite Kite

KiTe

Hare

HARE Hear hear keti keet keto <strong>Sample Output: </strong>

kite KiTe

KiTe Hare hare

……

……

KiTe

……

KiTe




<ol start="7">

 <li>Mess 1 is working on its menu list. After recent cases it has decided to create a dataset in which they are asking the patients of the most recent item they ate. Based on that they want to find the <strong><em>k</em></strong> most frequent dish resulting in food poisoning.</li>

</ol>

<strong>Note </strong>– Please answer in sorted order of frequency




<strong>Sample Input </strong>

6 (Number of patients)

Dosa

Dosa

Bread Butter

Pav bhaji

Pav bhaji

Poha

2




<strong>Sample Output </strong>

Dosa Pav bhaji




<ol start="8">

 <li>Hogwarts is under attack. Harry is making a Dumbledore army to fight back. He has arranged <strong><em>N</em></strong> people and he knows their current power levels. Now in this fight, combinations are very important. Given an array of power levels, find out whether there are two distinct indices <strong><em>i</em></strong> and <strong><em>j</em></strong> (<strong><em>1 &lt;= i, j &lt; N</em></strong>) in the array such that the absolute difference between <strong><em>power[i]</em></strong> and <strong><em>power[j]</em></strong> is at most <strong><em>t</em></strong> and the absolute difference between <strong><em>i</em></strong> and <strong><em>j</em></strong> is at most <strong><em>k</em></strong>. If the above conditions are satisfied, print “Hogwarts wins” or else print “Voldemort wins”. <strong>Note –</strong> Power level can also be a negative number.</li>

</ol>




<strong>Sample Input Format: <em>N k t </em></strong>

An array of <strong><em>N</em></strong> integers




<strong>Sample Input: </strong>

4 3 0

1 2 3 1




<strong>Sample Output: </strong>

Hogwarts Wins




<strong>Sample Input: </strong>

6 2 3

1 5 9 1 5 9

<strong>Sample Output: </strong>

Voldemort Wins




<ol start="9">

 <li>Given pre-order and in-order traversals of a binary search tree, construct the binary search tree. Output the post-order of the tree.</li>

</ol>




<strong>Note –</strong> You need to construct the tree and then print the post-order <strong>Note </strong>– You can assume that there are no duplicates




<strong>Sample Input Format: </strong>

<strong><em>N </em></strong>

In-order traversal

Pre-order traversal




<strong>Sample Input: </strong>

3

<ul>

 <li>2 3</li>

 <li>1 3</li>

</ul>




<strong>Sample Output: </strong>

2 3 1




<ol start="10">

 <li>You are the word master. The words are just too big for you. You decide to make a shortest possible unique prefix for every word.</li>

</ol>




<strong>Sample Input: </strong>

4 (Number of words)

Zebra

Dog

Duck

Dove




<strong>Sample Output: </strong>

Z

Dog Du

Dov







****************************