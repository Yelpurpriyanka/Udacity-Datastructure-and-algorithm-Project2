## 1. Problem Explanation on LRU caching 

Is basically a Linked List backed by a Hash table -> why?
* we want fast look up (that is what a hash table was needed)
* we want order and fast insertion (The need of a linked list)

Then Each node was being saved with the reference to the next and previous one into
the hash table, in that way we are able to look at a node without going through all
the linked list

Time and space complexity  are as follows
 * get --->  Time O(1), Space O(1) -> Our dictionary can access easily
 * set --->  Time O(1), Space O(1) -> We can add a new entry in O(1) thanks to self.head