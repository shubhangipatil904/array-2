# array-2
Programiz

Search Programiz

C# Arrays
In this tutorial, we will learn about C# arrays. We will learn to create, initialize, and access array with the help of examples.

An array is a collection of similar types of data. For example,

Suppose we need to record the age of 5 students. Instead of creating 5 separate variables, we can simply create an array:

Create an array that includes ages of 5 students
Elements of an Array
1. C# Array Declaration
In C#, here is how we can declare an array.

datatype[] arrayName;
Here,

dataType - data type like int, string, char, etc
arrayName - it is an identifier
Let's see an example,

int[] age;
Here, we have created an array named age. It can store elements of int type.

But how many elements can it store?

To define the number of elements that an array can hold, we have to allocate memory for the array in C#. For example,

// declare an array
int[] age;

// allocate memory for array
age = new int[5];
Here, new int[5] represents that the array can store 5 elements. We can also say the size/length of the array is 5.

Note: We can also declare and allocate the memory of an array in a single line. For example,

int[] age = new int[5];
2. Array initialization in C#
In C#, we can initialize an array during the declaration. For example,

int [] numbers = {1, 2, 3, 4, 5};
Here, we have created an array named numbers and initialized it with values 1, 2, 3, 4, and 5 inside the curly braces.

Note that we have not provided the size of the array. In this case, the C# automatically specifies the size by counting the number of elements in the array (i.e. 5).

In an array, we use an index number to determine the position of each array element. We can use the index number to initialize an array in C#. For example,

// declare an array
int[] age = new int[5];

//initializing array
age[0] = 12;
age[1] = 4;
age[2] = 5;
...
Initialize Array using the index number
C# Array Initialization
Note:

An array index always starts at 0. That is, the first element of an array is at index 0.
If the size of an array is 5, the index of the last element will be at 4 (5 - 1).
3. Access Array Elements
We can access the elements in the array using the index of the array. For example,

// access element at index 2
array[2];

// access element at index 4
array[4];
Here,

array[2] - access the 3rd element
array[4] - access the 5th element
Example: C# Array
using System;

namespace AccessArray
 {
  class Program 
 {
    static void Main(string[] args) 
{ 
      int[] numbers = {1, 2, 3}

     Console.WriteLine("Element in first index : " + numbers[0]);

     
      Console.WriteLine("Element in second index : " + numbers[1]);

      
      Console.WriteLine("Element in third index : " + numbers[2]);

      Console.ReadLine();

    }
  }
}
