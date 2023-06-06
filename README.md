# Inheritance

## Aim:
To write a C# program to print some messages using hierarchical inheritance

## Algorithm:
Step 1:
Create a base class.

Step 2:
Create two child class.

Step 3:
Create a constructor in the base class and print a message.

Step 4:
create a function in child class to print a message.

## Program:
~~~
using System;
namespace Autovechicle
{
    public class tyre
    {
        public tyre()
        {
            Console.WriteLine("Constructor tyre");
        }
        public virtual void Display()
        {
            Console.WriteLine("tyre");
        }
    }
    public class scooter : tyre
    {
        public scooter()
        {
            Console.WriteLine("Constructor sports car");
        }

        public override void Display()
        {
            base.Display();
            Console.WriteLine("sports car");
        }
    }

    public class car : tyre
    {
        public car()
        {
            Console.WriteLine("Constructor bike");
        }
        public override void Display()
        {
            base.Display();
            Console.WriteLine("bike");
        }
    }

    public class Program
    {
        public static void Main(string[] args)
        {
            car cd = new car();
            scooter cdd = new scooter();
            cd.Display();
            cdd.Display();
        }
    }
}
~~~

## Output:
![g1](https://github.com/Sharmilasha/Inheritance/assets/94506182/313def2e-c239-46df-aac9-0934aad57878)



## Result
Thus to create C# program to print some messages using hierarchical inheritance is implemented successfully.
