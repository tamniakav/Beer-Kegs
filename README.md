# Beer-Kegs
Just another repository
using System;

namespace _12.Beer_Kegs
{
    class Program
    {
        static void Main(string[] args)
        {
            int n = int.Parse(Console.ReadLine());
            string kegsName = string.Empty;
            double bigestKeg = 0;

            for (int i = 0; i < n; i++)
            {
                string typeOfKeg = Console.ReadLine();
                double r = double.Parse(Console.ReadLine());
                int h = int.Parse(Console.ReadLine());

                double sizeOfKeg = Math.PI * (r * r) * h;

                if (sizeOfKeg > bigestKeg)
                {
                    bigestKeg = sizeOfKeg;
                    kegsName = typeOfKeg;
                }
            }

            Console.WriteLine(kegsName);
        }
    }
}
