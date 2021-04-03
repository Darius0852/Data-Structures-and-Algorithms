# Data-Structures-and-Algorithms
Notes from Data Structures and Algorithms from courses/exercises

# Notes

## Intro to Data Structure and Algorithms

Data structure is a way of organising data in such a way that we can perform operations on these data in an effective way. Data structures is about rendering data elements in terms of some relationship, for better organization and storage. For example, we have some data which has, player's name "Virat" and age 26. Here "Virat" is a **String** data type and 26 is of **Integer** data type.

We can organize this data as a record like **Player** record, which will have both player's name and age in it. Now we can collect and store player's records in a file or database as a data structure. **For example**: "Dhoni" 30, "Gambhi" 31, "Sue" 35.

If you are aware of OO programming concepts, then a **class** also does the same thing, it collects differect types of data under one single entity. The only difference being, data structures provides for techniaues to access and manipulate data efficiently. 

In simple language, Data Structures are structures programmed to store ordered data, so that various oprations can be performed on it easily. It represents the knowledge of data to be organized by memory. It should be designed and implemented in such a way that it reduces complexity and increases efficiency.

## Basic Types of Data Structures

Anything that can store data can be called a data structure, hence Integer, Float, Boolean, Char ect, all are data structures. They are known as **Primitive Data Structures**.

Then we also have some complex Data Structres, which are used to store large and connected data. Some example of **Abstract Data Structures** are:
- Linked List
- Tree
- Graph
- Stack, Queue ect.

![](https://github.com/Darius0852/Data-Structures-and-Algorithms/blob/main/Images/introduction-to-data-structures.gif)

All these data structures allow us to perform different operations on data. We select these data structures based on which type of operation is required.

### Intro to Data Structures

Data structures can be classified on the basis of the following characteristics:

| Characteristic  | Description |
| :---            | :----:      |
| Linear          | In Linear data structures,the data items are arranged in a linear sequence. Example: **Array** |
| Non-Linear      | In Non-Linear data structures, the data items are not in sequence. Example: **Tree, Graph** |
| Homogeneous     | In homogeneous data structures, all the elements are of the same type. Example: **Array** |
| Non-Homogeneous | In Non-Homogeneous data structures, the elements may or may not be of the same type. Example **Structures** |
| Static          | Static data structures are those whose sizes and structures associated memory locations are fixed at compile time. Example: **Array** |
| Dynamic         | Dynamic structures are those which expands or shrinks depending upon the program need and its execution. Also, their associated memory locations changes. Example: **Linked List created using pointers** |


### What is an Algorithm ?

An algorithm is a finite set of instructions or logic, written in order to accomplish a certain predefined task. An Algorithm is not the complete code or program, it is just tge core logic (solution) of a problem, which can be expressed either as an informal high level description as **pseudocode** or using a **flowchart**.

Every Algorithm must satisfy the foloowing properties:

1. **Input** - There should be 0 or more inputs supplied externally to the algorithm.
2. **Output** - There should be atleast 1 output obtained.
3. **Definiteness** - Every algorithm should be clear and well defined.
4. **Finiteness** - The algorithm should have a finite number of steps. 
5. **Corectness** - Every steo of the algorithm must generate a correct output. 

An algorithm is said to be efficient and fast, if it takes less time to execute and consumes less memory space. The performance of the algorithm is measured on the basis of following properties:

1. Time Complexity
2. Space Complexity

### Space Complexity

Its the amount of memory space required by the algorithm, during the course of its execution. Space complexity must be taken seriously for multi-user systems and in situations where limited memory is availible. 

An algorithm generally requires space for following components:
- **Instruction Space**: Its the space required to store the executable version of the program. Thi space is fixed, but varies dependant upon the number of lines of code int he program. 
- **Data Space**: Its the space required to store all the constants and variable (including temporary variable) values.
- **Environment Space**: Its the space required to store the environment information needed to resume the suspended function.

### Time Complexity

Time Complexity is a way to represent the amount of time required by the program to run till its completion. It's generally a good practice to try to keep the time required minimum, so that our algorithm completes it's execution in the minimum time possible.

## Asymptotic Notations

When it comes to analysing the complexity of any algorithm in terms of time and space, we can never provide an exact number to define the time required and the space required by the algorithm, instead we express it using some standard notations, also known as **Asymptotic Notations**.

When we analyse any algorithm, we generally get a formula to represent the amount of time required for execution or the time required by the computer to run the lines of code of the algorithm, number of memory accesses, number of comparisons, temporary variables occupying memory space ect. This formula often contains unimportant details that don't really tell us anything about the running time. 

Let us take an example, if some algorithm has a time complexity of T(n) = (n<sup>2</sup> + 3n + 4), which is a quadratic equation. For large values of n, the 3n + 4 part will become insignificant compared to the n<sup>2</sup> part. 

Also, when we compare the execution times of two algorithms the constant coefficients of higher order terms are also neglected.

An algorithm that takes a time of 200n<sup>2</sup> will be faster than some other algorithm that takes n<sup>3</sup> time, for any value of n larger than 200. Since we're only insterested in the asymptotic behaviour of the growth of the function, the constant factor can be ignored too. 

## What is Asymptotic Behaviour

The word **Asymptotic** means approaching a value or curve arbitrarily closely (i.e., as some sort of limit is taken).

Remember studying about **Limits** in High School, this is the same. 

The only difference being, here we do not have to find the value of any expression where n is approaching any finite number or infinity, but in the case of Asymptotic notations, we use the same model to ignore the constant factors and insignificant parts of an expression, to devise a better way of representing complexities of algorithms, in a single coefficient, so that comparison between algorithms can be done easily. 

Let's take an example to understand this:

If we have two algorithms with the following expressions representing the time required by them for execution, then:

**Expression 1**: (20n<sup>2</sup> + 3n - 4)
**Expression 2**: (n<sup>3</sup> + 100n - 2)

Now, as per asymptotic notations, we should just worry about how the function will grow as the value of n (input) will grow, and that will entirely depend on n<sup>2</sup> for the Expression 1, and on n<sup>3</sup> for Expression 2. Hence, we can clearly say that the algorithm for which running time is represented by the Expression 2, will grow faster than the other one, simply by analysing the hihgest coefficient and ignoring the other constants (20 in 20n<sup>2</sup>) and insignificant parts of the expression (3n - 4 and 100n - 2).

The main idea behind casting aside the less important part is to make things manageable. All we need to do is, first analyse the algorithm to find out an expression to define it's time requirements and then analyse how that expression will grow as the input(n) will grow.

## Types of Asymptotic Notations

We use three types of asymptopic notations to represent the growth of any algorithm, as input increases:

1) Big Theta (Θ)
2) Big Oh (O)
3) Big Omega (Ω)

### Tight Bounds: Theta 

When we say tight bounds, we mean that the time complexity represented by the Big-O notation is like the average value or range within which the actual time of execution of the algorithm will be. 

For example, if for some algorithm the time complexity is represented by the expression 3n<sup>2</sup> + 5n, and we use the Big-Θ notation to represent this, then the time complexity would be Θ(n<sup>2</sup>) ignoring the constant coefficient and removing the insignificant part, which is 5n. 

Here, in the example above, complexity of Θ(n<sup>2</sup>) means, that the average time for any input n will remain in between k1 * n<sup>2</sup> and k2 * n<sup>2</sup>, where k1 and k2 are two constants, thereby tightly binding the expression representing the growth of the algorithm. 
