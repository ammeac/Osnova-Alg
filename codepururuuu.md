1.
  ```
using System;

class Program {
    static void Main() {
        string[] input = Console.ReadLine().Split();
        
        long a = Convert.ToInt64(input[0]);
        long b = Convert.ToInt64(input[1]);

        long totalTasks = a + b;
        

        Console.WriteLine(totalTasks);
    }
}
```

2.
  ```
﻿using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp3
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int a = Convert.ToInt32(Console.ReadLine());
            int b = Convert.ToInt32(Console.ReadLine());
            int c = Convert.ToInt32(Console.ReadLine());
            if (a + b > c && a + c > b && b + c > a)
            {
                Console.WriteLine("Да");
            }
            else
            {
                Console.WriteLine("Нет");
            }
        }
    }
}
  ```

3.
    ```
﻿using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp3
{
    internal class Program
    {
        static void Main(string[] args)
        {

            string[] numbers = Console.ReadLine().Split();
            int count = 0;

            for (int i = 1; i < numbers.Length - 1; i++)
            {

                if (Convert.ToInt64(numbers[i]) > Convert.ToInt64(numbers[i - 1]) && Convert.ToInt64(numbers[i]) > Convert.ToInt64(numbers[i + 1]))
                    count++;
            }

            Console.WriteLine(count);


        }
    }
}
  ```

4.
    ```
﻿using System;

namespace app4
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int number = int.Parse(Console.ReadLine());

            int[] fibonacciArray = new int[number + 1];

            fibonacciArray[1] = 1;

            if (number >= 2)
            {
                fibonacciArray[2] = 1;
            }

            for (int i = 3; i <= number; i++)
            {
                fibonacciArray[i] = fibonacciArray[i - 1] + fibonacciArray[i - 2];
            }
          
            int sumOfNumbers = 0;
            for (int i = 1; i <= number; i++)
            {
                sumOfNumbers = sumOfNumbers + fibonacciArray[i];
            }
            Console.WriteLine(sumOfNumbers);
        }
    }
}


  ```
5.
    ```
using System;

namespace ConsoleApp3
{
    internal class Program
    {
        static void Main(string[] args)
        {
            string[] input = Console.ReadLine().Split();
            int a = int.Parse(input[0]);
            int b = int.Parse(input[1]);
            int c = int.Parse(input[2]);

            double discriminant = (b * b) - (4 * a * c);

            if (discriminant == 0)
            {

                double root = -b / (2.0 * a);
                Console.WriteLine(root);
            }
            else
            {

                double sqrtDiscriminant = Math.Sqrt(discriminant);

                double root1 = (-b + sqrtDiscriminant) / (2 * a);
                double root2 = (-b - sqrtDiscriminant) / (2 * a);

                Console.WriteLine(root1 + " " + root2);
            }
        }
    }
}

  ```
