using System;
using System.Text;

namespace RandomPasswordGenerator
{
  class Program
  {
    static void Main(string[] args)
    {
       
      int i = 0;
      int total = 0; // متغیر جدید برای جمع قیمت غذا ها
      int a=0;//متغییر جدید برای ضرب قیمت پیتزا و تعداد
	  int b=0;//متغییر جدید برای ضرب قیمت پاستا و تعداد
	  int c=0;//مغییر جدید برای ضرب قیمت نوشیدنی و تعداد
	  int d=0;//متغییر جدید برای ضرب قیمت سالاد و تعداد
	  int Pi=0;//گرفتن تعداد پیتزا
	  int Be=0;//گرفتن تعداد پاستا
	  int Pa=0;//گرفتن تعداد نوشیدنی
	  int Sa=0;//گرفتن تعداد سالاد
	  
      for (i = 1; i < 5; i++)
   {
    Console.ForegroundColor=ConsoleColor.White;
	Console.BackgroundColor=ConsoleColor.Red;
    Console.WriteLine("      what do you want?  ");
	Console.Beep(200,800);
    Console.WriteLine("      [1]Pizza           ");
	Console.Beep(200,800);
    Console.WriteLine("      [2]Pasta           ");
	Console.Beep(200,800);
    Console.WriteLine("      [3]Beverages       ");
	Console.Beep(200,800);
    Console.WriteLine("      [4]Salad           ");
	Console.Beep(200,800);
    Console.WriteLine("      [5]Receipt         ");
	Console.Beep(200,800);
    Console.WriteLine("      Choose a category: ");
	Console.Beep(200,800);
    string choice = Console.ReadLine();
	
    Console.Clear();
	
    switch (choice)
    {
        // پیتزا
        case "1":
		    Console.ForegroundColor=ConsoleColor.Black;
	        Console.BackgroundColor=ConsoleColor.White;
            Console.WriteLine(" [1]pepperoni                    12000");
			Console.Beep(400,800);
            Console.WriteLine(" [2]mixed                        12000");
			Console.Beep(400,800);
            Console.WriteLine(" [3]theVegetables                12000");
			Console.Beep(400,800);
            Console.WriteLine(" [4]MushroomsAndChicken          12000");
			Console.Beep(400,800);
            Console.WriteLine(" What kind of pizza do you want?      ");
			Console.Beep(400,800);
            int Pizza = int.Parse(Console.ReadLine());
            Console.WriteLine("how many do you want?                 ");
			Console.Beep(400,800);
            Pi = int.Parse(Console.ReadLine());//دریافت تعداد
            a = (Pi * 12000);//قیمت نهایی
            total += a; // جمع قیمت پیتزا به متغیر total اضافه می‌شود
            Console.WriteLine(a);
			Console.Beep(400,800);
			Console.Clear();
            break;

        // پاستا
        case "2":
		    Console.ForegroundColor=ConsoleColor.Black;
	        Console.BackgroundColor=ConsoleColor.White;
            Console.WriteLine("  [1]BeefRicottaFettuccine        30000");
			Console.Beep(400,800);
            Console.WriteLine("  [2]PenneBeefAlfredo             30000");
			Console.Beep(400,800);
            Console.WriteLine("  [3]TandooriChickenAlfredo       30000");
			Console.Beep(400,800);
            Console.WriteLine("  [4]TandooriBeefAlfredo          30000");
			Console.Beep(400,800);
            Console.WriteLine("  What kind of pasta do you want?      ");
			Console.Beep(400,800);
            string Pasta = Console.ReadLine();
            Console.WriteLine("  how many do you want?                ");
			Console.Beep(400,800);
            Pa = int.Parse(Console.ReadLine());//دریافت تعداد
            b = (Pa * 30000);// قیمت نهایی  
            total += b; // جمع قیمت پاستا به متغیر total اضافه می‌شود
            Console.WriteLine(b);
			Console.Beep(400,800);
			Console.Clear();
            break;

        // نوشیدنی
        case "3":
		    Console.ForegroundColor=ConsoleColor.Black;
	        Console.BackgroundColor=ConsoleColor.White;
            Console.WriteLine("  [1]softDrinks                   5000");
			Console.Beep(400,800);
            Console.WriteLine("  [2]Coffee                       5000");
			Console.Beep(400,800);
            Console.WriteLine("  [3]mojito                       5000");
			Console.Beep(400,800);
            Console.WriteLine("  [4]OrengJoice                   5000");
			Console.Beep(400,800);
            Console.WriteLine("  What type of drink do you want?     ");
			Console.Beep(400,800);
            int Beverages = int.Parse(Console.ReadLine());
            Console.WriteLine("  how many do you want?               ");
			Console.Beep(400,800);
            Be = int.Parse(Console.ReadLine());//دریافت تعداد
            c = (Be * 5000);//قیمت نهایی
            total += c; // جمع قیمت نوشیدنی به متغیر total اضافه می‌شود
            Console.WriteLine(c);
			Console.Beep(400,800);
			Console.Clear();
            break;

        // سالاد
        case "4":
		    Console.ForegroundColor=ConsoleColor.Black;
	        Console.BackgroundColor=ConsoleColor.White;
            Console.WriteLine("  [1]Caesar                       9000");
			Console.Beep(400,800);
            Console.WriteLine("  [2]Macaroni                     9000");
			Console.Beep(400,800);
            Console.WriteLine("  [3]Chicken                      9000");
			Console.Beep(400,800);
            Console.WriteLine("  [4]Waldorf                      9000");
			Console.Beep(400,800);
            Console.WriteLine("  What kind of salad do you want?     ");
			Console.Beep(400,800);
            int Salad = int.Parse(Console.ReadLine());
            Console.WriteLine("  how many do you want?               ");
			Console.Beep(400,800);
            Sa = int.Parse(Console.ReadLine());//دریافت تعداد
            d = (Sa * 9000);//قیمت نهایی
            total += d; // جمع قیمت سالاد به متغیر total اضافه می‌شود
            Console.WriteLine(d);
			Console.Beep(400,800);
			Console.Clear();
            break;
			
	    //رسید
        case "5":
		    Console.ForegroundColor=ConsoleColor.White;
	        Console.BackgroundColor=ConsoleColor.DarkRed;
	    	Console.WriteLine("  Pizza     {0}      {1}      ",Pi,a);//نمایش تعداد و قیمت نهایی پیتزا
			Console.Beep(400,800);
	        Console.WriteLine("  Pasta     {0}      {1}      ",Pa,b);//نمایش تعداد و قیمت نهایی پاستا
			Console.Beep(400,800);
	        Console.WriteLine("  Beverages {0}      {1}      ",Be,c);//نمایش تعداد و قیمت نهایی نوشیدنی
			Console.Beep(400,800);
	        Console.WriteLine("  Salad     {0}      {1}      ",Sa,d);//نمایش تعداد و قیمت نهایی سالاد
			Console.Beep(400,800);
            Console.WriteLine("  Total price:       {0}      " ,total);//نمایش قیمت کل
			Console.Beep(400,800);
		    break;
			
        default:
            Console.WriteLine("Errore");//در صورتی اجرا میشود که کاربر عددی را اشتباه وارد کند
			Console.Beep(800,800);
            break;
    }
    
   }

    }
  }
}
