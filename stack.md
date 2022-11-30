# Stacks
# 📌 A Brief Overview

Stacks are a built in collection that allows us to store data. 

Stacks are great for data that is meant to be stored temporarily. It is very easy and efficent to edit a stack. However, stacks store data in LIFO or Last In First Out style. This means that if we have a stack of `ABCD` the first thing we have to remove is `D` and work from there.

Lets see a stack in action before diving deeper.

```csharp
// Create
var myStack = new Stack<int>(0, 1, 2, 3, 4);

// Remove
int lastNumber = myStack.Pop();

// Add
int numberToAdd = 99;
myStack.Add(numberToAdd);
```

Our `myStack` is now going to be `0, 1, 2, 3, 99`. Because we removed the last and added a new one to the end.

# 📚 Our Little Library
Let's say that we have a stack of books. 
![Stack of books](images/bookStack.png)

We will be using this stack today to learn more about this datastructure. Yay!

Stacks are another kind of datastructure that allows us to store data, add to it, remove it, and read it.




# 🏫 Creating the Library
## Creating an Empty Stack

To create an empty stack you are going to create a variable for your stack and then set that equal to an instance of the built in stack including the data type. 

Lets see it in action.

```csharp
// Format:
// [variable Type] [Variabe Name] = new Stack<[datatype]>();

Stack<string> Library = new Stack<string>();
```
## Creating a stack that contains elements
To create a stack that is already filled with things you place what you want to be in the stack inside the parenthesis
```csharp
// Format:
// [variable Type] [Variabe Name] = new Stack<[datatype]>(elements);

Stack<string> Library = new Stack<string>("To Kill a Mockingbird", "The Kite Runner", "Forever");
```


# Stack Methods
Now that we have a stack created, we can look at a few of the methods and properties built into the stack class
## _ _ _ _ _ _ _ _ _  
## Push()
## Pop()
## Clear()
## .Contains
## _ _ _ _ _ _ _ _ _ _

## Adding Books - Push()
We can add elements to our stack by using the `Push` function. This appends a new element to the __top__ of the stack. 

We can push onto empty stacks and stacks that already contain items
```csharp
// Format: 
// [Stack Name].Push([what is being added]);

Library.Push("To Kill a Mockingbird");
Library.Push("The Kite Runner");
Library.Push("Forever");
Library.Push("The Adventures of Huckleberry Finn");
```
`Push()` adds an item to the top of the stack so with the code that we have made our stack if it was empty before will look like this...

<img src="images/first4.png" alt="smaller stack of books" width="400"/>

## Removing Books - Pop()
Because stacks use the last in first out model. When we remove a book or "pop it off" we are taking from the top of our stack. 

So this code:

```csharp
// Format: 
// [Stack Name].Pop();

Library.Pop();
```
will remove the top book "The Adventures if huckleberry Finn". Leaving us with this...

<img src="images/first3.png" alt="smaller stack of books" width="300"/>


# Example Problems
Write the code for the following scenario. In the back of a classroom is a stack of books that the students have read each semester. The stack at the moment looks like this. 
![starting stack](images/bookStack.png)

Jeremy wants to read "Harry Potter and the socereres stone". To get to this book he will create a new smaller stack on the floor one book at a time and then add them back
