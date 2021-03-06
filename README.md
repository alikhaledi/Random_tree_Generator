# Random_tree_Generator
This Matlab program is written by Ali Khaledi-Nasab @Ohio_University 
Here we generate random tree networks using 4 different types of branchings. 
The main program is "Tree_Generator_main.m"
Once you open this program, you can choose among 4 types of branchings. 

1. Full_Binary_Branching: The branching is m2=2 until generation 2, and it is either 0 or 2. The probability of zero branching is p0. 

2. General_Binary_Branching: The zero branching for the root is either 1 or 2, and for the rest, it is 0, 1, or 2. p(m1)=p0, p(m1)=p(m2)=(1-p0)/2

3. Uniform_Branching: Zero branching is allowed after the second generation thus the branching at the root is (1-nd). 
For the rest, it is (0-nd). The branching is generated using uniform random numbers. 

4. Binomial_Branching: Zero branching is allowed after the second generation thus the branching at the root is (1-nd). 
For the rest, it is (0-nd). The branching is generated using Binomial random numbers with p=p0, and n=nd, B(nd,p0).  

There are two more functions in the folder: 

adjacency_matrix_generator: Generate the adjacency matrix for a given branching array,B, and the maximum allowed generation,ng.

Save_adjacency2file: will save a thee tree along with its total number of nodes and the total number of heminodes. as following :

node 
nh
A(1,1)
A(1,2)
.
.
.
A(1,n)
A(2,1)
.
.
.
A(node,node)

The file name will be file_number.tree
If you are interested to save the random trees, uncomment line 22 in the main program (Tree_Generator_main).
