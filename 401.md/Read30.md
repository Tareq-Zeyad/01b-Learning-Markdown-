# Hash Tables
![hash](https://i2.wp.com/techvidvan.com/tutorials/wp-content/uploads/sites/2/2021/07/TechVidvan-Hash-Table.jpg?fit=1200%2C628&ssl=1)
### What is a Hashtable? 

- In computing, a hash table is a data structure that implements an associative array abstract data type, a structure that can map keys to values. A hash table uses a hash function to compute an index, also called a hash code, into an array of buckets or slots, from which the desired value can be found.

### What are the common terminologies for hashtables ?


1. Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
2. Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
3. Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.



### Why do we use Hashtables ?

- To:
1. Hold unique values
2. Dictionary
3. Library


### What is mainly the idea of Hashtables ?

- The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value. This is done through what we call a hash. A hash is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value. Since we are able to hash our key and determine the exact location where our value is stored, we can do a lookup in an O(1) time complexity. This is ideal when quick lookups are required.


### How can we create a hash ?

- A hashtable traditionally is created from an array. I always like the size 1024. this is important for index placement. After you have created your array of the appropriate size, do some sort of logic to turn that “key” into a numeric number value. Here is a possible suggestion:

Add or multiply all the ASCII values together.
Multiply it by a prime number such as 599.
Use modulo to get the remainder of the result, when divided by the total size of the array.
Insert into the array at that index.

- Example:
```
Key = "Cat"
Value = "Josie"

67 + 97 + 116 = 280

280 * 599 = 69648

69648 % 1024 = 16
```

Key gets placed in index of 16. 
We now know that our key Cat maps to index 16 of the array. We can view into this index and find “Josie”, our value quickly.


### What do hashmaps do to store values ?

- Hash maps do this to store values:

accept a key
calculate the hash of the key
use modulus to convert the hash into an array index
store the key with the value by appending both to the end of a linked list

### What do hashmaps do to read a value ?

- Hash maps do this to read value:

accept a key
calculate the hash of the key
use modulus to convert the hash into an array index
use the array index to access the short LinkedList representing a bucket
search through the bucket looking for a node with a key/value pair that matches the key you were given.