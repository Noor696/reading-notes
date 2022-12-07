## Hashtables

[Hashtables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)

* hashtable, it is used to determine the index of the array.

* Buckets ,Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

* Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

------

* Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.

* The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value. This is done through what we call a **hash**

* in arrays We using a **for loop** that looks through each piece of data one by one until it finds the specific item, This would be an O(N) read operation because it requires searching through each piece of data to find the one piece we want. 
--> 
* Arrays actually have fast access. If we know the index of the information we want we can access that information in O(1) time.

* a hash map uses a “hash function” to place each item at a precise index location, based off it’s key.

* Hashing: a hash code turns a key into an integer. their output is determined only by their input, The same key should always produce the same hash code.

* Bucket Sizes: Hash Maps can have any number of buckets. If a hash map has only a few buckets it will be densely full and have many collisions. If a hash map has more buckets it will be more sparsely populated, there will be less collisions, but there may be a lot of extra empty space.

* Hash maps do this to store values:

  - accept a key
  - calculate the hash of the key
  - use modulus to convert the hash into an array index
  - store the key with the value by appending both to the end of a linked list

* Hash maps do this to read value:

  - accept a key
  - calculate the hash of the key
  - use modulus to convert the hash into an array index
  - use the array index to access the short LinkedList representing a bucket
  - search through the bucket looking for a node with a key/value pair that matches the key you were given