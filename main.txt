using System;
namespace od2
{
    class Program
    {
        static void Main(string[] args)
        {
            ///Bir konsol uygulamasında kullanıcıdan pozitif iki sayı girmesini isteyin (n, m). 
            /// Sonrasında kullanıcıdan n adet pozitif sayı girmesini isteyin. Kullanıcının girmiş olduğu 
            /// sayılardan m'e eşit yada tam bölünenleri console'a yazdırın.


            Console.WriteLine("Lütfen pozitif iki sayı giriniz:");
            int diziUzunlugu =int.Parse(Console.ReadLine());
            int sayi =int.Parse(Console.ReadLine());
            int[] dizi = new int[diziUzunlugu];
            
            for (int i = 0; i < diziUzunlugu; i++)
            {
                Console.WriteLine("Lütfen {0}. sayıyı giriniz " ,i+1);
                dizi[i] = int.Parse(Console.ReadLine());
            }

            foreach (var sayilar in dizi)
            {
                //if(sayilar == sayi || sayilar/sayi ==0 )

                if ( sayilar == sayi || sayi%sayilar == 0)
                Console.WriteLine(sayilar);
            }

        }
    }
}