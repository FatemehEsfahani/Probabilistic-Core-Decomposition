# K-Core Decomposition of Large Probabilistic Graphs
This repository contains efficient implementations for computing the k-core decomposition of large probabilistic graphs. The details of the implementations are described in the following paper:

Fatemeh Esfahani, Venkatesh Srinivasan, Alex Thomo, and Kui Wu: Efficient Computation of Probabilistic Core Decomposition at
Web-Scale. In Proceedings of the 22nd International Conference on Extending Database Technology (EDBT), 325–336. 

# K_BZ
This is an implementation of core decomposition for probabilistic graphs using WebGraph compression framework in:

P. Boldi and S. Vigna. The webgraph framework I: compression techniques. WWW'04

# K_VC
This is an implementation of core decomposition for probabilistic graphs, which do not fit in main memeory, using WebGraph compression framework in:

P. Boldi and S. Vigna. The webgraph framework I: compression techniques. WWW'04

# Input for K_BZ and K_VC
The graphs for K_BZ and K_VC should be in WebGraph format with edges being assigned probabilities.

There are three files in this format:

newTest.w.labeloffsets

newTest.w.labels

newTest.w.properties

(see simplegraph example in the main directory)


# Compiling

<pre>
mkdir -p bin; javac -cp "bin":"lib/*" -d bin src/it/unimi/dsi/webgraph/labelling/*.java src/*.java
</pre>

# Using git
First clone repo.

<pre>
git clone https://github.com/thomouvic/pcore.git
</pre>

This will create a directory "pcore" with the current code of this project. The subdirectories created are "src" and "lib". 

Copy the source files you changed to "pcode/src". 

While being in "pcode", run 
<pre>
git add .
</pre>

Commit changes by running
<pre>
git commit -m "some comment about your changes"
</pre>
If it is the first time, you will be required to run two other commands before. 
<pre>
git config --global user.email "your email"
git config --global user.name "your name"
</pre>

Finally, run
<pre>
git push
</pre>

You will be required to specify username and password. 
If successful, the changes will be in the repository.

