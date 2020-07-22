Author: Liam Axon

----DESCRIPTION OF HOMOLOGY----
In case you don't know what homology is, it is a way of assigning
groups to (in this case) simplicial complexes. It is a theorem that two
simplicial complexes which have the same underlying topological space
will have the same homology groups, and because of this, homology groups
are especially useful for differentiating topological spaces.


----EXPLANATION OF THE PROGRAM----

This is a program to create simplicial complexes (of dimension at most 3), and to determine their homology groups.
Additionally, this lets you compute the homology of a sub-complex and the relative homology with respect to that sub-complex,
which gives you the Long Exact Sequence in homology.

There are also a few pre-made simplicial complexes, such as the 3-sphere or the Klein Bottle

Most buttons are explained with tool tips, which also gives their keyboard hotkeys.
However, I list them here just in case:
Q: select
W: add
E: delete
R: add square
T: move point
Y: assign a point
U: split a point
A: add to the main complex
S: remove from the main complex
F: move in the world
G: name a point
Z: add to the sub-complex
X: remove from the sub-complex
C: add all selected to the sub-complex
V: add all simplices equivalent to the sub-complex that are equivalent to one in the sub-complex
SPACE: pause / unpause

-----ORGANIZATION OF THE CODE-----

The program was written in Eclilpse. The program's GUI is designed using Java Swing, with the help of the WindowBuilder tool. 
The program is organized into three packages.
    windowstuff contains all files having to do with Java Swing components.
        In particular, it contains SimplexExplorer.class, which is the main file from which everything runs
    simplicialcomplexes contains all files having to do with simplices and simplicial complexes.
    chaincomplexes contains all files having to do with finitely generated abelian groups and chain complexes
        In fact, chaincomplexes has the tools to create and manipulate any finitely generated abelian group,
        and to handle any finite chain complex made out of these groups.

The main function is found in windowstuff/Start.class