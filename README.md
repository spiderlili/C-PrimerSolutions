# CppPrimerSolutions
C++ Primer Solutions

### Why does the built-in array not support the assignment of one array with another? What information is required to support this operation?<br>

C++ only provide limited support to the mechanics required to read and write individual elements.C++ does not support the abstraction of an array - there is no supoprt for the assignment of one array to another, the comparison of two arrays for equality or asking an array its size. To assign one array to another, copy each element in turn and program this:<br>

for (int index = 0; index < 10, ++index)
  array0[index] = array1[index]

### What operations should a first class array support?
A C++ array is not a first-class citizen of the language: it is inherited form the C language and reflects the separation of data and the algorithms that operate on that data that are characteristic of the procedural paradigm. <br>
First class operations typically include being passed as an argument, returned from a function, modified, and assigned to a variable.<br>
The C++ array type has no self-knowledge and does not know its size, so must keep track of this independently of the array itself - this becomes troublesome when wanting to pass arrays as general arguments to functions.
