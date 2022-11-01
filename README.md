### EX NO : 06
### DATE  : 12.05.2022
# <p align="center">Operator-Overloading</p>


## Aim:
 To write a C# program to find the volume of a box using operator overloading
 
 ## Algorithm:
## Step 1:
 Create a class for operator overloading.

## Step 2:
Get inputs for length,breadth from the user in overloading function.

## Step 3:
Compare the inputs such as length and breadth.

## Step 4:
Using equal to(==) and not equal to(!=) operator we can compare the inputs.

## Step 5:
Print the result.

 ## Program:
 ```
 using System;

namespace OperOverload
{
   class Program
   {
       int n;
       public Program(int a)
       {
           this.n = a;
           Console.WriteLine("This is a parameterized constructor");
           Console.WriteLine("The value is " + this.n);
       }
       public Program()
       {
           this.n = 12;
           Console.WriteLine("This is a default constructor \n The value is " + this.n);
       }
       public static bool operator ==(Program p1, Program p2)
       {
           return p1.Equals(p2);
       }
       public static bool operator !=(Program p1, Program p2)
       {
           return !p1.Equals(p2);
       }
       static void Main(string[] args)
       {
           Program p1 = new Program(12);
           Program p4 = new Program();
           Program p2=p4;
           if (p2 == p4)
           {
               Console.WriteLine("They both are equal");
           }
           else if (p1 != p4)
           {
               Console.WriteLine("They both are different ");
           }
       }
   }
}
 ```
 ## Output:
 ![image](12.jpg)
 
 ## Result:
C# program using operator overloading is implemented successfully.
