# Big O Notation

### What is the need for Big O Notation?
* To compare performance of different implementations of an algorithm. Big O provides a trend for how the number of operations scale for running the algorithm as the scale of the input increases
* There are two aspects of performance
  * Time complexity - Reflects how the execution duration scales with the size of the input
  * Space complexity - Reflects how the memory required scales with the size of the input

### Simplifying Big-O expressions
* Rule of thumbs for Big O expressions
  * Constants don't matter - O(2n) ~ O(n), O(500) ~ O(1)
  * Big O shorthands
    * Arithmetic operations are constants
    * Variable assignment is constant
    * Accessing elements in an array (by index) or object (by key) is constant
    * In a loop the complexity is the length of the loop times the complexity of whatever happens inside of the loop
    
### Space complexity
* Auxiliary space complexity - The space/ memory taken up by the algorithm not including the space taken up by the inputs
* Rules of thumb when calculating space complexity
  * Most primitives (booleans, numbers, undefined) are constant space
  * Strings require O(n) space where n is the length of the string
  * Reference types are generally O(n) where n is the length (for arrays) or the number of keys (for objects)
   
### Logarithmic complexity
* Certain searching algorithms have logarithmic time complexity
* Efficient sorting algorithms involve logarithms
* Recursion sometimes involves logarithmic space complexity
