# Train
Train 
using System;

namespace Train
{
    class Program
    {
        static void Main(string[] args)
        {
            int num = int.Parse(Console.ReadLine());// from here we take the lenght of the array

            int[] numbers = new int[num];// we create the array and it has the length of the wagons (input from the console)

            // filling the array with numbers of passangers for each wagon

            int sum = 0; //here we initiate the sum of all passangers

            // we create for loop to go through the whole lenght of the array and we will fill 
            //every single index with the input from the console.

            for (int i = 0; i < numbers.Length; i++) 
            {
                // here we start to fill our wagons with passengers, numbers[i] gives us access to the current numnber of passangers
                numbers[i] = int.Parse(Console.ReadLine());
                sum += numbers[i]; // here we add to the sum the numbers of the passangers every time we read a number

            }

            // we passed through all the numbers of passangers and now we have our current arrays.
            //we start with foreach loop to go through all the collection of arrays
            // we print all the elements on a single row

            //!!! When the loop is finished (false) we proceed to the foreach loop and print the results:


            foreach (int number in numbers)
            {
                Console.Write(number + " ");
            }

            Console.WriteLine(); // here we put an empty row
            Console.Write(sum);
        }

            
    }
}
