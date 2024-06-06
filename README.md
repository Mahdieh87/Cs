using System;
using System.Text;

namespace RandomPasswordGenerator
{
  class Program
  {
    static void Main(string[] args)
    {
      Console.ForegroundColor=ConsoleColor.White;
      Console.BackgroundColor=ConsoleColor.Red;
	  
	  //حلقه
	  int i=0 ;
	  for (i=1;i<2;i++)
	  //منوی اصلی
	{ Console.WriteLine("what do you want?");
      Console.WriteLine("Pizza");
      Console.WriteLine("Pasta");
      Console.WriteLine("Beverages");
      Console.WriteLine("Salad");
	  
      Console.WriteLine(" Choose a category: ");
      string choice = Console.ReadLine();
	  
      switch (choice)
     {
      //پیتزا
      case "Pizza":
      Console.WriteLine("[1]pepperoni                    12000");
	  Console.WriteLine("[2]mixed                        12000");
	  Console.WriteLine("[3]theVegetables                12000");
	  Console.WriteLine("[4]MushroomsAndChicken          12000");
	  Console.WriteLine("What kind of pizza do you want?");
	  int Pizza=int.Parse(Console.ReadLine());
	  Console.WriteLine("how many do you want?");
	  int Pi=int.Parse(Console.ReadLine());
	  int a=(Pi*12000);
	  Console.WriteLine(a);
	  
      break;
	  
	  //پاستا
      case "Pasta":
      Console.WriteLine("[1]BeefRicottaFettuccine        30000");
	  Console.WriteLine("[2]PenneBeefAlfredo             30000");
	  Console.WriteLine("[3]TandooriChickenAlfredo       30000");
	  Console.WriteLine("[4]TandooriBeefAlfredo          30000");
	  Console.WriteLine("What kind of pasta do you want?");
	  string Pasta=Console.ReadLine();
	  Console.WriteLine("how many do you want?");
	  int Pa=int.Parse(Console.ReadLine());
	  int b=(Pa*30000);
	  Console.WriteLine(b);
	  
	  break;
	  
	  //نوشیدنی
      case "Beverages":
      Console.WriteLine("[1]softDrinks                   5000");
	  Console.WriteLine("[2]Coffee                       5000");
	  Console.WriteLine("[3]mojito                       5000");
	  Console.WriteLine("[4]OrengJoice                   5000");
	  Console.WriteLine("What type of drink do you want?");
	  int Beverages=int.Parse(Console.ReadLine());
	  Console.WriteLine("how many do you want?");
	  int Be=int.Parse(Console.ReadLine());
	  int c=(Be*5000);
	  Console.WriteLine(c);
	  
      break;
	  
	  //سالاد
      case "Salad":
      Console.WriteLine("[1]Caesar                       9000");
	  Console.WriteLine("[2]Macaroni                     9000");
	  Console.WriteLine("[3]Chicken                      9000");
	  Console.WriteLine("[4]Waldorf                      9000");
	  Console.Write("What kind of salad do you want?");
	  int Salad=int.Parse(Console.ReadLine());
	  Console.Write("how many do you want?");
	  int Sa=int.Parse(Console.ReadLine());
	  int d=(Sa*9000);
	  Console.WriteLine(d);
	  
      break;
	  
      default:
      Console.WriteLine("Errore");
      break;
	  }
	 }
	 
	 
    }
  }
}
