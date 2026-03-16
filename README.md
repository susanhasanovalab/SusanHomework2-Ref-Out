# SusanHomework2-Ref-Out

//EV TaPSIRIGI 2
//1.1


////using System;

////class Program
////{
////    static void Susan(ref int[] arr, int value)
////    {
////        for (int i = 0; i < arr.Length; i++)
////        {
////            arr[i] += value;
////        }
////    }

////    static void Camila(int[] arr)
////    {
////        foreach (int num in arr)
////        {
////            Console.Write(num + " ");
////        }
////        Console.WriteLine();
////    }

////    static void Main()
////    {
////        int[] numbers = { 1, 1, 33, 43, 51 };

////        Console.WriteLine("Metoddan evvel");
////        Camila(numbers);

////        Susan(ref numbers, 3);

////        Console.WriteLine("Metoddan sonra");
////        Camila(numbers);
////    }
////}




//1.2
//using System;

//class Program
//{
//    static void Withdraw(ref double balance, double amount)
//    {
//        if (balance >= amount)
//        {
//            balance = balance - amount;
//        }
//        else
//        {
//            Console.WriteLine("Not enough balance");
//        }
//    }

//    static void Main()
//    {
//        double balance = 100000000;

//        Console.WriteLine("Balance before: " + balance);

//        Withdraw(ref balance, 40767868);

//        Console.WriteLine("Balance after: " + balance);
//    }
//}




//1.3
//using System;

//class Program
//{
//    static void GetMinMax(int[] arr, out int min, out int max)
//    {
//        min = arr[0];
//        max = arr[0];

//        for (int i = 0; i < arr.Length; i++)
//        {
//            if (arr[i] < min)
//            {
//                min = arr[i];
//            }

//            if (arr[i] > max)
//            {
//                max = arr[i];
//            }
//        }
//    }

//    static void Main()
//    {
//        int[] numbers = { 5, 2, 9, 1, 7 };

//        int min;
//        int max;

//        GetMinMax(numbers, out min, out max);

//        Console.WriteLine("Minimum: " + min);
//        Console.WriteLine("Maximum: " + max);
//    }
//}



//1.4

//using System;

//class Program
//{
//    static bool ProcessNumber(ref int number, out bool isEven)
//    {
//        number = number + number;

//        if (number % 2 == 0)
//        {
//            isEven = true;
//        }
//        else
//        {
//            isEven = false;
//        }

//        return isEven;
//    }

//    static void Main()
//    {
//        int number = 5;
//        bool isEven;

//        ProcessNumber(ref number, out isEven);

//        Console.WriteLine("New number: " + number);
//        Console.WriteLine("Is even: " + isEven);
//    }
//}




//2.1

//using System;
//class Product
//{
//    public string Name;
//    public double Price;

//    public void ShowInfo()
//    {
//        Console.WriteLine("Name: " + Name);
//        Console.WriteLine("Price: " + Price);
//    }
//}

//class Book : Product
//{
//    public string Author;

  
//    public new void ShowInfo()
//    {
//        Console.WriteLine("Name: " + Name);
//        Console.WriteLine("Price: " + Price);
//        Console.WriteLine("Author: " + Author);
//    }
//}

//class Program
//{
//    static void Main()
//    {
//        Book book = new Book();
//        book.Name = "BioInformatics";
//        book.Price = 2500;
//        book.Author = "Susan Hasanova";
//        book.ShowInfo();
//    }
//}
