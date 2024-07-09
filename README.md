using System;
using System.Globalization;
using System.Runtime.InteropServices;

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            //Task_1.........................................................
            //Console.Write("Enter First Number:");
            //string first = Console.ReadLine();
            //int num1 = int.Parse(first);
            //Console.Write("Enter second Number:");
            //string second = Console.ReadLine();
            //int num2 = int.Parse(first);
            //sum(num1,num2);

            //Task_2.........................................................

            //int A = 2;
            //even(A);

            //Task_3.........................................................
            /*Console.Write("Enter an year:");
            string year = Console.ReadLine();
            int num1 = int.Parse(year);
            Leapyear(num1);*/

            //Task_4.........................................................

            //double speed = 1000; // (km/hr)
            //milesperhr(speed);

            //Task_5.........................................................

            //int num = 27;
            //buzz(num);

            //Task_6.........................................................
            
            Console.Write("which table you want:");
            string num1 = Console.ReadLine();
            int num = int.Parse(num1);
            table(num);
            
            //Task_7.........................................................
            /*int num = 3;int fact=num; int C = 1;
            while (num > 0) { C=C*num; num--; }
            Console.WriteLine($"factorail of {fact}! is {C}");
            */
            //Task_8.........................................................
            //int A = 2;
            //int B = A-1;
            //bool isprime = true;
            //while (B != 1)
            //{
            //    if (A % B == 0)
            //    {
            //        isprime = false;
            //    }
            //    B = B - 1;
            //}
            //if (isprime == true)
            //{
            //    Console.Write("it is a prime number");
            //}
            //else
            //{
            //    Console.Write("it is not a prime number");

            //}

            //Task_9.........................................................
            /* int A = 10;
             int B = 20;
             int C = 10;
             if (A == B && B == C) { Console.Write($"it is equilateral triangle"); }
             if(A == B || B == C || A==C) { Console.Write($"it is isosceles triangle"); }
             else { Console.Write($"it is scalene triangle"); }
             */
            //Task_10.........................................................
            /*int i = 1;
            while (i <= 5) {
                int j = 1;
                while (j <= i) {
                    Console.Write("*");
                    j++;
                }
                Console.Write("\n");
                i++;
                    }*/
            //Bonous Task.........................................................
            //int A = 121;
            //palin(A);

        }
        //Task_1............................function.............................
        static void sum(int num1, int num2)
        {
            int sum = num1 + num2;
            Console.WriteLine($"sum of two numbers is :{sum}");

        }
        //Task_2............................function.............................
        static void even(int A)
        {
            while (A <= 100)
            {
                Console.Write($" {A}");
                A = A + 2;
            }

        }
        //Task_3............................function.............................
        static void Leapyear(int year)
        {
            int check = year % 4;
            if (check == 0)
            { Console.WriteLine("This is a leap year"); }
            else { Console.WriteLine("This is not a leap year"); }
        }
        //Task_4.........................................................
        static void milesperhr(double speed)
        {
            double B = speed * 0.621371; ;
            Console.Write($"The speed in miles/hr is: {B}");
        }
        //Task_5.........................................................
        static void buzz(int num)
        {
            int modulus = num % 7;
            int avaliable = num % 10;
            if (modulus == 0 || avaliable == 7)
            { Console.Write($"Number {num} is a buzz number"); }
            else { Console.Write($"Number {num} is not a buzz number"); }
         
        }
        //Task_6.........................................................
        static void table(int num)
        {
            int i = 1;
            while (i <= 10)
            { int mult = num * i; Console.Write($"{num} X {i} = {mult}\n"); i++; }
        }
        //Bonous............................function.............................
        static void palin(int num)
        {
            int cat = num;
            int rev = 0;
            int K = 0;
            while (num != 0)
            {
                int Digit = num % 10;
                rev = (rev * 10) + Digit;
                num = num / 10;
            }
            if (cat == rev)
            {
                Console.Write("it is a Palindrome");
            }
            else { Console.Write("it is not a Palindrome"); }

        }
    }
}
