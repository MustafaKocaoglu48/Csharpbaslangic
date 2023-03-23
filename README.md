# Csharpbaslangic
---
### Ekrana yazdırma
````
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace İlk_uygulama1
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
            Console.ReadKey();
        }
    }
}

````
### Veri tiplerine değişken atama
````
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
            int tam_sayi = 5;
            double ondalikli_sayi=23.4;
            string isim = "Mustafa";
            char karakter = 'A';
            Boolean ifade=false;
            float ondalikli = 23.4f;

        }
    }
}
````
### Konsoldan veri alma 
````
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
            int sayi;
            Console.WriteLine("Lütfen bir sayı giriniz.");
            sayi=Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Girilen sayi: " + sayi);

            string isim;
            Console.WriteLine("Lütfen bir string değer giriniz:");
            isim = Console.ReadLine();
            Console.WriteLine("Girilen string: " + isim);

            char karakter;
            Console.WriteLine("Lütfen bir karakter giriniz");
            karakter=Convert.ToChar(Console.ReadLine());
            Console.WriteLine("Girilen karakter:" + karakter);

            Boolean deger;
            Console.WriteLine("Lütfen bir boolean değer giriniz:");
            deger= Convert.ToBoolean(Console.ReadLine());
            Console.WriteLine("Girilen değer:" + deger);

            
            Console.ReadLine(); ;

        }
    }
}
````
### Klavyeden girilen 2 sayının toplamı
````
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
            Console.WriteLine("Lütfen toplama işlemi için ilk sayıyı giriniz.");
            int ilk_sayi=Convert.ToInt32(Console.ReadLine());

            Console.WriteLine("Lütfen toplama işlemi için 2. sayıyı giriniz");
            int ikinci_sayi = Convert.ToInt32(Console.ReadLine());

            int toplam = ilk_sayi + ikinci_sayi;
            Console.WriteLine("Girilen sayıların toplamı:" + toplam);
            
            Console.ReadLine(); ;

        }
    }
}
````
### İki sayının toplamı
````
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
            int ilk_sayi = 10;
            int ikinci_sayi=20;
            int toplam = ilk_sayi + ikinci_sayi;
            Console.WriteLine("Sayıların toplamı:" + toplam);
            Console.ReadLine(); ;

        }
    }
}

````
### Vize ve final notuna göre genel ortalama hesaplayan program
````
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
            Console.WriteLine("Lütfen vize notunuzu giriniz:");
            int vize = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Lütfen final notunuzu giriniz:");
            int final= Convert.ToInt32(Console.ReadLine());

            double ortalama = vize * 0.4 + final * 0.6;
            Console.WriteLine("Genel ortalamanız:" + ortalama);
            Console.ReadLine(); ;

        }
    }
}

````
