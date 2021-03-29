# Data-Structures-and-Algorithms
Notes from Data Structures and Algorithms from courses/exercises

# Notes

## Intro to Data Structure and Algorithms

Data structure is a way of organising data in such a way that we can perform operatioons on these data in an effective way. Data structures is about rendering data elements in terms of some relationship, for better organization and storage. For example, we have some adat which has, player's name "Virat" and age 26. Here "Virat" is a **String** data type and 26 is of **Integer** data type.

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
