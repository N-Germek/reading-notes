# Data Structures and Algorithms

## Important things to consider when deciding data structures to solve problems

> The best way to determine which data structure to use would be to first identify how much compound data you have to work with and how you will need to use it.

If using recursion, be aware of the base case and the recursive case.  The recursive case is when the function calls itself, the base case is when the function doesn’t call itself.
The amount of compound data determines the speed at which processing can happen.

### Types of Data Structures

The linked list is a list form of data structure, it contains a node (the atomic unit). The node contains the value and a pointer, the first of which is the head and the last of which is the tail. Pros to linked lists are that they are good at adding and removing nodes. Cons are that they are only aware of the nodes next to them so retrieval and searching is limited.

The array data structure stores data at specific locations. Since each item in an array has a location, the ability to retrieve or search for specific data is made easier since all data is aware of the other data in the array. Cons to using an array, is that adding items to robust arrays can make them more time consuming to search for in the future.

The hash table is the object in JavaScript or the dictionary (dict) in python. If you search the key in Python with a hashing function, it will give you the definition which translates into the value of that object.  Cons are the instances of collisions in which multiple keys will have the same hash value and require different ways to identify which data you are intending to locate.  Pros are the ability to add, remove and retrieve data.

Stack and Queue are similar data structures. The stack is a last in first out data structure, to access you would need to push(1) items in or pop() them out.  The call stack is important to know so you can make algorithms appropriate to the data needed to be retrieved.  The Queue is the first in first out data structure. Similar to a line at a store, customers are helped in the order that they came into the line.   To add or remove data to a queue, you would use .enqueue(1) or .dequeue(). The algorithm bread first search or bfs is primarily used for these.

Graphs and Trees are similar to linked lists with nodes and edges which can have weights assigned to them. Trees have a more one directional structure, yet they can also contain more data in a more relative method. The binary search tree is an example of a method to very specifically search for data in a large tree structure. The rules are as follows:
Each node can have 0-2 children
The left node can only be smaller than the parent node while the right node can only be larger than the parent node.

## Ways to Avoid an Infinite Recursive Call Stack

> In recursive call stacks, the best way to avoid an infinite loop, you will want to have a solid base case function that stops the loop once the conditions are met. This way the function will have a way to stop calling itself.

### What is Big O

O(1) (O of 1) is the way that we describe the constant time for transferring data.
O(N) (O of N) is how the internet transfers data in linear time where N is the amount of data. N is just a variable and can be renamed to whatever variable makes sense.

## Things I want to know more about

I learned that control + c ends an infinite loop in many programs.  I would like to learn all the codes to end infinite loops in different developer tools since those tend to be some of the things that I spend the most time debugging in my own code.

### Resources

> [Recursion in software development](https://www.youtube.com/watch?v=vPEJSJMg4jY)

> [DATA STRUCTURES you MUST know(as a Software Developer)](https://www.youtube.com/watch?v=sVxBVvlnJsM)

> [Big O Notation](https://www.youtube.com/watch?v=v4cd1O4zkGw)

### Links

> [Advanced Software Development](README.md)
