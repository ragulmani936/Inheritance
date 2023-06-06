# Inheritance

## Aim:

To write a C# program to print some messages using hierarchical inheritance

## Algorithm:

### Step1:
Create a base class.

### Step2:
Create two child class.

### Step3:
Create a constructor in the base class and print a message.

### Step4:
create a function in child class to print a message.


## Program:
~~~
Developed by: Ragul M
Reg no: 212221230080
~~~
~~~
using System;
namespace Autovechicle
{
    public class tyre
    {
        public tyre()
        {
            Console.WriteLine("Tyre Constructor");
        }
        public virtual void Display()
        {
            Console.WriteLine("Method in tyre class");
        }
    }
    public class scooter : tyre
    {
        public scooter()
        {
            Console.WriteLine("Scooter Constructor");
        }

        public override void Display()
        {
            base.Display();
            Console.WriteLine("Method in Scooter");
        }
    }

    public class car : tyre
    {
        public car()
        {
            Console.WriteLine("Car Constructor");
        }

        public override void Display()
        {
            base.Display();
            Console.WriteLine("Method in Car");
        }
    }
    public class Program
    {
        public static void Main(string[] args)
        {
            scooter s = new scooter();
            s.Display();
            car c = new car();
            c.Display();
        }
    }
}
~~~

## Output:

![img1](https://github.com/ragulmani936/Inheritance/blob/main/img%201.png)

## Result:
Thus C# program to print some messages using hierarchical inheritance is written and executed sucessfully.
