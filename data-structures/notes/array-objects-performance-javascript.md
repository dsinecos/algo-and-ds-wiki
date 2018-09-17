# Comparing performance of Arrays vs Objects in JavaScript (from the Big-O lens)
    
### Reference - [JS Algorithms and Data Structures - Section 3](https://www.udemy.com/js-algorithms-and-data-structures-masterclass/learn/v4/t/lecture/11198324?start=0)
    
### Objectives
* Understand how objects and arrays work through the lens of BigO
* Explain why adding elements to the beginning of an array is costly
* Compare and contrast the runtime for arrays and objects

## Objects

#### When to use objects
* When you don't need any order among the key-value pairs
* When you need fast access/ insertion and removal
    * Insertion - O(1)
    * Removal - O(1)
    * Access - O(1)
    * Searching - O(N) - Accessing a key is achieved in constant time, however searching for a value that might be against any key, has O(N) complexity

#### Runtime complexity for various object methods
* `Object.keys` - O(N)
* `Object.values` - O(N)
* `Object.entries` - O(N)
* `hasOwnProperty` - O(1)

## Arrays

#### When to use arrays
* When you need to store data as an ordered list
* When you need fast access/ insertion and removal
    * Access - O(1)
    * Searching - O(N)
    * Insertion/ Removal - Depends
        * Adding/ Removing at the end of an array - O(1)
        * Adding/ Removing at the beginning of an array - O(N) where N is the size of the array into which an element is inserted because all the elements have to be reindexed
        * Push and Pop are always faster than Shift and Unshift

#### Runtime complexity for various Array Methods
* `push` and `pop` - O(1)
* `shift` and `unshift` - O(N)
* `concat`, `slice` and `splice` - O(N)
* `sort` - O(N*logN)
