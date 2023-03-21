# Pattern

## Aim:
To write a C# program for a pascal's triangle.
## Equipment Required:
Microsoft Visual Studio 2022
## Algorithm:
```
1.Start the program.
2.Get the limit from the user.
3.Use for loop to print the rows , columns and space.
4.Use if-else condition inside the loop to print the values.
5.Use c = c * (i - j + 1) / j to print the inner value.
6.Using Console.write print the Pascal's triangle.
7.End the program
```

## Program:
```
using System;
namespace PascalTriane
{
    public class pascalPattern
    {
        public static void Main(string[] args)
        {
            int rows, i, j,k, count = 1;
            Console.Write("Enter the numbers for rows: ");
            rows = Convert.ToInt32(Console.ReadLine());
            for (i = 0; i < rows; i++)
            {
                for (j = 1; j <= rows - i; j++)
                {
                    Console.Write(" ");
                }
                for (k = 0; k<=i; k++)
                {
                    if (i == 0 || k == 0)
                    {
                        count = 1;
                    }
                    else
                    {
                        count = count * (i - k + 1) / k;
                    }
                 Console.Write("{0} " , count);
                }
                Console.Write("\n");
            }
  
        }
    }
}
```

## Output:
![O](https://github.com/dharanielango/C-Pattern/blob/main/c%233.png)

## Result:
 Thus,C# program for a pascal's triangle is executed successfully.
