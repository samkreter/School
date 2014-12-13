Hash Tabls
==========
- All cases O(1) time

**Load Facetor** - a = n/m where
- n is the number of elements in the array
- m is the number of slots 

Red Back Tree's
===============
###Insertion###
**Parent is black** - everything is fine. done

**Case 1: Parent and Uncle are red**
- make grandparent red
- parent and uncle black
- move z to its grandparent 

**Case 2: Parent is red and is left child of grandparent, uncle is black z is right child**
- left rotate parent
- z becomes right child

**Case 3: Parent is red and is left child of grandparent, uncle is black z is right child**
- make parent black and grandparent red
- right rotate on grandparent
- everything is good 

###Deletion###
**complecated deletion**
- if x points to root everythings good no worries
- if x points to red node then change it black and everything is fixed
- if x ponits to black node then 
--* testing this