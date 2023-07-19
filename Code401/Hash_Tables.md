# Hashtables

**A hashtable** is a data structure that stores key-value pairs using a hash function to determine the index where the value is stored. This allows for fast retrieval of values in constant time. The purpose of a hashtable is to hold unique values and provide efficient lookup operations.

To create a hashtable, an array is typically used, and the keys are converted into numeric values through a hashing algorithm. The hash code is then used to determine the index in the array where the key-value pair should be stored. Collisions can occur when different keys produce the same hash code, which is resolved by storing the pairs in linked lists within the buckets of the array.

The hashtable provides methods such as: 

**1. set()**

When adding a new key/value pair to a hashtable:

  send the key to the hash() method.
  Once you determine the index of where it should be placed, go to that index
  Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
  If something does exist, add the new key/value pair to the data structure within that bucket.

**3. get()**

The get() method takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.

**5. has()**
   
The has() method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the hash() method and check the hashtable if the key exists in the table given the index returned.

**7. keys()**
   
The keys() method returns a collection (array) of unique hash keys.

**9. hash()**
    
The hash() method will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed.
