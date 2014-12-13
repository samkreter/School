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

**Parent and Uncle are red**
- make grandparent red
- parent and uncle black
- move z to its parent 

**Parent is red and is left child of grandparent**
- left rotate parent