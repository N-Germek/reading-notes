# Stacks and Queues

## Terminology

Push - To put nodes or objects into a stack.
Pop - To remove nodes or items that are removed from the stack.    When the stack is empty, an exception is raised if you attempt to pop something out.
Top - Top of stack
Peep - To view the value of the top Node in the stack. When the stack is empty, an exception is raised if you attempt to peek at something that doesn’t exist.
IsEmpty - is the method to check if the stack is empty.  Boolean return.

## Stack Concepts

FILO - First In Last Out.
This means that the first item added to the stack will be the last item popped out of the stack.

LIFO - Last In First Out.
This means that the last item added to the stack will be the first item popped out of the stack.

Visualization for stacks is usually up and down, top to bottom.

### Push O(1)

Pushing will always be a O(1) because it take the same amount of time no matter the nodes you have in a stack. To push the node in, you add it to the top of the stack.

Steps to do this:
Have the node you want to add at the ready. Assign the next property to the current node assigned to the top.

```python
new_node = Node(value)
new_node.next = node_at_the_top
top = new_node
```

Here is an example of the pseudo code:

```python
ALOGORITHM push(value)
// INPUT <-- value to add, wrapped in Node internally
// OUTPUT <-- none
   node = new Node(value)
   node.next <-- Top
   top <-- Node
```

## Things I want to learn more about

## Resources

- > [Stacks and Queues](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)

## Links

- >[Advanced Software Development](README.md)
