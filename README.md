# What I Learned in Week 12

## Week 12 was about methods, setters, getters, classes, stacks, queues.

### Methods
A method is a function that is stored within an object.  Methods are meant to allow you to manipulate and work with the object that the method is of.  Here's an example array object with a method that returns the length of the array:
```
const myObject = {
    favNum: function() {
        return 123;
    }
};

myObject.favNum(); // 123
```

### Setters and Getters
Setters and getters are special functions that are called upon the reading or writing of a member variable.  they allow you to have more control over your objects and what data they can accept.

#### Getter example
```
const myObject = {
    get rand() { // Return number between 1 and 10
        return Math.floor(Math.random() * 10) + 1;
    }
};

myObject.rand; // Number between 1 and 10
```

#### Setter example
```
const myObject = {
    number: 2,
    set num(input) {
        this.number = input;
    }
};

myObject.number; // 2
myObject.num = 5;
myObject.number; // 5
```

### Stacks
A Stack is a FILO (First in, last out) data structure.  The two operations for a stack are `push` and `pop`.  When you `push` an item onto a stack, you add an item on top.  When you `pop` an item, you remove it.

```
const myStack = [];
myStack.push(1);
myStack.push(2);
myStack.push(3);
myStack;        // [1, 2, 3]
myStack.pop();  // 3
myStack.pop();  // 2
myStack.pop();  // 1
```

### Queues
A queue is a FIFO (first in, first out) data structure.  The two operations for a queue are `push` and `shift`.  You add items to the end with `push` and retrieve them from the beginning with `shift`.

```
const myQueue = [];
myQueue.push(1);
myQueue.push(2);
myQueue.push(3);
myQueue;
myQueue.shift(); // 1
myQueue.shift(); // 2
myQueue.shift(); // 3
```