using System;

class Program
{
    static void Main()
    {
        // Set console color
        Console.ForegroundColor = ConsoleColor.Cyan;
        
        // Display welcome message and menu
        Console.WriteLine("# WELCOME TO MY PROGRAM");
        Console.WriteLine("==========================");
        Console.WriteLine("\nPlease choose one of the option below\n");
        Console.WriteLine("1. Developer's name's first three letter");
        Console.WriteLine("2. Addition");
        Console.WriteLine("3. Absolute value of the subtraction");
        Console.WriteLine("4. Multiplication");
        Console.WriteLine("5. Exit");
        
        // Get user input
        Console.Write("\nWrite your option please: ");
        int choice = int.Parse(Console.ReadLine());
        
        // Process user choice
        if (choice == 1)
        {
            ShowDeveloperName();
        }
        else if (choice == 2)
        {
            PerformAddition();
        }
        else if (choice == 3)
        {
            PerformSubtraction();
        }
        else if (choice == 4)
        {
            PerformMultiplication();
        }
        else if (choice == 5)
        {
            // Just exit
        }
        else
        {
            Console.WriteLine("\nYou entered something other than a menu number");
        }
        
        // Thank you message
        Console.WriteLine("\nTHANK YOU and GOOD BYE");
    }
    
    static void ShowDeveloperName()
    {
        Console.WriteLine("\nMy name's first three letter\n");
        
        // Big letter 'A' (replace with your first initial)
        Console.WriteLine("  AA   BBBB  CCC ");
        Console.WriteLine(" A  A  B   B C   ");
        Console.WriteLine("AAAAA  BBBB  C   ");
        Console.WriteLine("A    A B   B C   ");
        Console.WriteLine("A    A BBBB  CCC");
        
        // Note: Replace the letters above with your own initials
        // This example shows A-B-C, you should change to your initials
    }
    
    static void PerformAddition()
    {
        Console.Write("\nPlease enter the first number: ");
        double num1 = double.Parse(Console.ReadLine());
        
        Console.Write("Please enter the second number: ");
        double num2 = double.Parse(Console.ReadLine());
        
        double result = num1 + num2;
        Console.WriteLine($"\nTotal of {num1} and {num2} is {result}");
    }
    
    static void PerformSubtraction()
    {
        Console.Write("\nPlease enter the first number: ");
        double num1 = double.Parse(Console.ReadLine());
        
        Console.Write("Please enter the second number: ");
        double num2 = double.Parse(Console.ReadLine());
        
        double result = Math.Abs(num1 - num2);
        Console.WriteLine($"\nDifference of {num1} and {num2} is {result}");
    }
    
    static void PerformMultiplication()
    {
        Console.Write("\nPlease enter the first number: ");
        double num1 = double.Parse(Console.ReadLine());
        
        Console.Write("Please enter the second number: ");
        double num2 = double.Parse(Console.ReadLine());
        
        double result = num1 * num2;
        Console.WriteLine($"\nMultiplication of {num1} and {num2} is {result}");
    }
}
