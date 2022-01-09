# NidaK-l-c


Örnek 1: Birbirinden farklı olarak verilen iki adet sayıdan, büyük olanı bulup gösteren java kodu:
package ikisayıdanbuyukolan;
import java.util.Scanner;
public class İkiSayıdanBuyukOlan { 
    public static void main(String[] args) {

           int sayi1,sayi2;// sayisal değerde iki değişken tanımlıyoruz.
        Scanner oku=new Scanner(System.in);
        System.out.println("Lütfen kıyaslanacak ilk sayiyi giriniz.");
        sayi1=oku.nextInt();
        System.out.println("Lütfen kıyaslanacak ikinci sayiyi giriniz");
        sayi2=oku.nextInt();
        if(sayi1>sayi2)
        {
            System.out.println("Büyük olan sayi:"+sayi1);  
      }
        else
            System.out.println("Büyük olan sayi"+sayi2);

    }
    
}




Örnek 2: Girilen vize ve final notlarına göre öğrencinin dersten geçip geçmediğini bulan java kodu:


package sinavortalaması;

import java.util.Scanner;

public class SinavOrtalaması {

    public static void main(String[] args) {
         Scanner reader = new Scanner(System.in);
        int vizeNot,finalNot;
        double ortalama;
        String durum="";
        System.out.print("Vize Notunuzu Girin : ");
        vizeNot=reader.nextInt();
        System.out.print("Final Notunuzu Girin : ");
        finalNot=reader.nextInt();
        ortalama=vizeNot*0.4+finalNot*0.6;
        if(ortalama>=50 && finalNot>=50){
            durum="Geçti";
        }
        else{
            durum="Kaldı";
        }
        System.out.println("Ortalama : " + ortalama);
         System.out.println("Durumunuz: " + durum); }    
}


Örnek 3: Verilen tamsayının  pozitif ya da negatif olup olmadığını bulan java kodu:
 package pozitifnegatif;
public class PozitifNegatif {
    public static void main(String[] args) {
        
                java.util.Scanner scanner = new java.util.Scanner(System.in);
                int sayi;
	System.out.println("Sayi giriniz:");
        sayi=scanner.nextInt(); //Klavyeden giriş istiyoruz
	  if(sayi>0) //Eğer ki girilen sayı 0'dan büyükse, sayı pozitiftir
	    System.out.println("Girilen sayi POZITIF");	
 
	  else //Eğer ki girilen sayı 0'dan küçükse, sayı negatiftir
	    System.out.println("Girilen sayi NEGATIF") ;
}


    }










Örnek 4: 1’den 50’ye kadar tek sayıları yazdıran java kodu:

package birelli;
public class BirElli {
    public static void main(String[] args) {
             int toplam=0;
        for(int i=1;i<=50;i++){
        if(i%2!=0){
           
          toplam += i;
        }
                }
        System.out.print("\n");
        System.out.println("Toplam="+toplam);
    }
}

    









Örnek 5: Beş sayının ortalamasını veren programa ait java kodu:

package bessayıtoplamı;
import java.util.Scanner;
public class BesSayıToplamı {

    public static void main(String[] args) {
             Scanner klavye=new Scanner(System.in);
        System.out.println("ilk sayiyi giriniz: ");
          int sayi1 = klavye.nextInt();
        System.out.println("İkinci sayiyi giriniz: ");
        int sayi2 = klavye.nextInt();
        System.out.println("Üçüncü sayiyi giriniz: ");
        int sayi3 = klavye.nextInt();
        System.out.println("Dördüncü sayiyi giriniz: ");
        int sayi4 = klavye.nextInt();
        System.out.println("Beşinci sayiyi giriniz: ");
        int sayi5 = klavye.nextInt();
        int toplam=sayi1+sayi2+sayi3+sayi4+sayi5;
        double ortalama=toplam/5.0;
        System.out.println("Bu 5 sayinin ortalamasi: "+ortalama);
   }
    }




Örnek  6: Kullanıcı tarafından girilen iki sayının bölümünün kalan sayıyı yazdıran java kodu:

package kalansayı;

import java.util.Scanner;

public class KalanSayı {

    public static void main(String[] args) {
             
        Scanner reader = new Scanner(System.in);
        System.out.print("Birinci Sayıyı Girin: ");         
        int sayi = reader.nextInt();
        System.out.print("İkinci Sayıyı Girin: ");   
        int bolen = reader.nextInt();
 
        int bolum = sayi / bolen;
        int kalan = sayi % bolen;
 
        System.out.println("İşlem:"+sayi+"/"+bolen + " : " +bolum);
        System.out.println("kalan : " + kalan);

    }
    
}


Örnek  7: Java İkinci Dereceden Denklemin Köklerini Bulma

 import java.util.Scanner;
 
 
public class JavaOrnekleri {
  
    public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in); 
        System.out.println("(ax²+bx+c) ikinci dereceden bir denklemdir.\n Denklemdeki sabitleri aşağıdaki gibi sırayla girin"); 
        
        System.out.print("a değerini giriniz :"); 
        double a = sc.nextInt(); 
        System.out.print("b değerini giriniz   :"); 
        double b = sc.nextInt(); 
        System.out.print("c değerini giriniz   :"); 
        double c = sc.nextInt(); 
        //diskriminant (delta)
        double delta = (b * b) - (4 * a * c); 
        
        if (delta > 0){ 
            double x1 = ((-1 * b) - Math.sqrt(delta)) / (2 * a); 
            double x2 = ((-1 * b) + Math.sqrt(delta)) / (2 * a); 
            System.out.println("x1= " + x1 + " x2= " + x2); 
        } 
        if (delta < 0){
            System.out.println("Denklemin Gerçel Kökü Yoktur."); 
        } 
        if (delta == 0){ 
            double x = (-1 * b) / (2 * a);
            System.out.println("Çakışık kökü var x1= x2= " + x); 
        }
 
    } 
}




Örnek 8:  n! değerini hesaplayan java kodu:
package faktoriyelhesabı;

import java.util.Scanner;

 class FaktoriyelHesabı {

 
    public static void main(String[] args) {
     Scanner scan = new Scanner(System.in);
        System.out.println("Sayi Giriniz : ");
        int deger = scan.nextInt();
        int faktoriyel = 1;
        for(int i = 1; i<= deger; 
                i++){
            faktoriyel = faktoriyel * i;
        }
         
        System.out.println(faktoriyel);
    }
}







Örnek9:Dikdörtegen çevresi ve alanı bulduran java kodu:

Soru9. package dikdörtgen;
import java.util.Scanner;
public class Dıkdortgen {
public static void main(String[] args) {
Scanner scan = new Scanner(System.in);
int kenar1,kenar2;System.out.print("1. Kenarı giriniz: ");
kenar1 = scan.nextInt();
System.out.print("2. Kenarı giriniz: ");kenar2 = scan.nextInt();
		
System.out.println("Dikdörtgenin alanı = " + (kenar1 * kenar2));
System.out.println("Dikdörtgenin çevresi = " + (2 * (kenar1 + kenar2)));
	}










Örnek10:Ebob ekok bulduran java kodu:

package ebobekok;

public class EbobEkok {

    public static void main(String[] args) {
             int n1 = 48, n2 = 160,ebob=1, ekok;
 
       for(int i = 1; i <=  n1 && i <= n2; ++i)
        {
            if(n1 % i == 0 && n2 % i == 0)
                ebob = i;
        }
 
        ekok = (n1 * n2) / ebob;
        System.out.printf(" %d ve  %d sayılarının EBOB'u %d \n", n1, n2, ebob);
        System.out.printf(" %d ve  %d sayılarının EKOK'u %d \n", n1, n2, ekok); 

        
    }
    
}
