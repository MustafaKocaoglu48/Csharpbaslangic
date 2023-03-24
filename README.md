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
### Klavyeden alınan ürün fiyatına göre kdvli fiyatı ekrana yazan program.
````
using System;


namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
            double kdvli_fiyat, normal_fiyat;
            Console.WriteLine("Lütfen ürünün fiyatını giriniz:");
            normal_fiyat=Convert.ToDouble(Console.ReadLine());
            kdvli_fiyat = 0.18 * normal_fiyat + normal_fiyat;
            Console.WriteLine("Ürünün kdvli fiyatı:" + kdvli_fiyat);

        }
    }
}
````
### Klavyeden girilen değerleri klavyeden girilen değerlere göre 4 işlem yapan program.
````
using System;


namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
            Console.WriteLine("Lütfen bir sayı giriniz:");
            double ilk_sayi=Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Lütfen ikinci bir sayı daha giriniz:");
            double ikinci_sayi = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Lütfen yapmak istediğiniz işlemi seçiniz:" +
                "1-Toplama" +
                "2-Çıkarma" +
                "3-Çarpma" +
                "4-Bölme");
            double secilen=Convert.ToInt32(Console.ReadLine());
            if (secilen == 1)
            {
                Console.WriteLine("İşleminizin sonucu:"+ilk_sayi + ikinci_sayi);

            }else if (secilen == 2)
            {
                Console.WriteLine("İşleminizin sonucu:" +(ilk_sayi-ikinci_sayi));
            }else if(secilen == 3) { 
            Console.WriteLine("İşleminizin sonucu:" + ilk_sayi *ikinci_sayi);
            }
            else
            {
                Console.WriteLine("İşleminizin sonucu:" + ilk_sayi / ikinci_sayi);
            }

        }
    }
}

````
### While döngüsü ile adımızı 10 defa ekrana ayzan program.
````

using System;


namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
            int i = 0;
            while(i<10)
            {
                Console.WriteLine("Mustafa");
                i++;
            }
            Console.ReadLine();
        }
    }
}

````
### do-While döngüsü ile adımızı 10 defa ekrana ayzan program.
````
using System;


namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
            int i = 0;
            do
            {
                Console.WriteLine("Mustafa");
                i++;
            } while (i < 5);
            Console.ReadLine();
        }
    }
}
````
### for döngüsü ile adımızı ekrana 10 defa yazan program.
````
using System;


namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
          for(int i=0;i<10;i++)
            {
                Console.WriteLine("Mustafa");
            }
            Console.ReadLine();
        }
    }
}

````
### 1-100 arasında 7 ile bölünebilen sayıları ekrana yazan program
````
using System;


namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
          for(int i=1;i<100;i++)
            {
                if (i % 7 == 0)
                {
                    Console.WriteLine(i);
                }
            }
            Console.ReadLine();
        }
    }
}
````
### 1-20 arasındaki sayıların toplamını bulan program
````
using System;


namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
            int toplam = 0;
          for(int i=1;i<=20;i++)
            {
                toplam += i;
            }Console.WriteLine(toplam);
            Console.ReadLine();
        }
    }
}
````
### Klavyeden girilen 20 adet sayının toplamını veren program
````
using System;


namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
            int toplam = 0;
          for(int i = 0; i < 20; i++)
            {
                int sayi=Convert.ToInt32(Console.ReadLine());
                toplam += sayi;
            }Console.WriteLine(toplam);
            Console.ReadLine();
        }
    }
}

````
### Klavyeden girilen 10 adet sayının çift olanları yazan ve kaç adet olduğunu bulan program
````
using System;
namespace İlk_uygulama1
{
    internal class Program
    {
          static void Main(string[] args)
        {
            int toplam = 0;
          for(int i = 0; i < 10; i++)
            {
                int sayi=Convert.ToInt32(Console.ReadLine());
                if (sayi % 2 == 0)
                {
                    Console.WriteLine(sayi);
                }
              
            }
            Console.ReadLine();
        }
    }
}
````


