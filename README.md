# C#
# Factorial
# method

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace star
{
    class Program
    {      
        static int Factorial(int n)
        {
            if (n == 0)
            {
                return 1;
            }

            return n * Factorial(n-1); 
        }

        static void Main(string[] args)
        {
            int n;
            Console.WriteLine("자연수 입력: ");

            string input = Console.ReadLine();
            bool isParseOk = int.TryParse(input, out n);
            
	Console.WriteLine(Factorial(n));

            Console.ReadKey(true);
            
        }
    }
}
