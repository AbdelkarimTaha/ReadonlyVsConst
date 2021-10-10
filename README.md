# ReadonlycVsConst
Difference between readonly and const keyword in C#

const keyword is used to declare constant fields and constant local. The value of the constant field is the same throughout the program or in other words, once the constant field is assigned the value of this field is not be changed. In C#, constant fields and locals are not variables, a constant is a number, string, null reference, boolean values.


Example:
--------
class GFG {
 
    // Constant fields
    public const int myvar = 10;
    public const string str = "GeeksforGeeks";
 
    // Main method
    static public void Main()
    {
        // Display the value of Constant fields
        Console.WriteLine("The value of myvar: {0}", myvar);
        Console.WriteLine("The value of str: {0}", str);
    }
}

Output: 
-------
The value of myvar: 10
The value of str: GeeksforGeeks
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------
you can use a readonly keyword to declare a readonly variable. This readonly keyword shows that you can assign the variable only when you declare a variable or in a constructor of the same class in which it is declared.

Example:
--------
class GFG {
 
    // readonly variables
    public readonly int myvar1;
    public readonly int myvar2;
 
    // Values of the readonly
    // variables are assigned
    // Using constructor
    public GFG(int b, int c)
    {
        myvar1 = b;
        myvar2 = c;
        Console.WriteLine("Display value of myvar1 {0}, " + "and myvar2 {1}", myvar1, myvar2);
    }
 
    // Main method
    static public void Main()
    {
        GFG obj1 = new GFG(100, 200);
    }
}

Output: 
-------
Display value of myvar1 100, and myvar2 200





