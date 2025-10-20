using System;

namespace ThemeParkCalculationTask
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Welcome to the Theme Park Ticket Calculator");
            Console.Write("Enter the number of people in your group: ");
            int numberOfPeople = Convert.ToInt32(Console.ReadLine());
            const decimal ticketPrice = 15m;
            const decimal groupDiscount = 5m;
            decimal totalCharge = numberOfPeople * ticketPrice;
            if (numberOfPeople >= 6)
            {
                totalCharge -= groupDiscount;
            }
            Console.WriteLine($"\nTotal charge for {numberOfPeople} people: £{totalCharge}")
        }
    }
}

Welcome to the Theme Park Ticket Calculator
Enter the number of people in your group: 4

Total charge for 4 people: £6


Welcome to the Theme Park Ticket Calculator
Enter the number of people in your group: 10

Total charge for 10 people: £145

Welcome to the Theme Park Ticket Calculator
Enter the number of people in your group: 6

Total charge for 6 people: £85
