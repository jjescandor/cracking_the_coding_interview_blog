### Hash Tables
- A hash table is a data structure that map keys to values for highly efficient lookup.
- There are different number of ways of implementing this
- In our implementation, we use an array of linked lists and a hash code function. 
- To insert a key, (which might be a string or essentially any data type) and value, we do the following
    - First compute the key's hash code, which will usually be an int or long. Note that two different keys, could have the same hash code, as there might be an infinite number of keys and a finite number of ints.
    - Then, map the hash code to an index in the array. This could be done with something like hash(key) % array_length. Two different hash code could map to the same index.
    - At this index, there is a linked lists of keys and values. Store the keys and values in this index. We must use a linked lists because of collisions. you could have two different keys with the same hash code or two different hash codes that map to the same index.

