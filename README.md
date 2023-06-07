# Recursive-function

##Aim: To write a C# program to reverse a number using recursive function.

##Algorithm:
### step 1 :
Create a function for reversing.
### step 2 :
Get the number from the user.
### step 3 :
In the function find reminder of the number and multiply it by 10 and add the reverse number.
### step 4 :
Recusively call this function to get the reversed number.
### step 5:
print the reversed number.
##Program:
~~~
Developed by : Meiyarasi.V
Register number : 212221230058
~~~
~~~
using System;
namespace Recursive_Function
{
    class Program
    {
        public static int m, reverse = 0;
        public static int Recur(int number)
        {
            
            if (number > 0)
            {
                Program.m = number % 10;
                Program.reverse = Program.reverse * 10 + m;
                number = number / 10;
                return Recur(number);
            }
            return Program.reverse;

        }
        static void Main(string[] args)
        {
            int num;
            num = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine(Recur(num));
        }
    }
}
~~~

##Output:
![image](https://github.com/21005984/Recursive-function/assets/94748389/a3bd980a-add5-475e-b483-53277d948a0e)

##Result:
Create a function for reversing.
