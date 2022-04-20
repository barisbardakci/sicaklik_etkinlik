# sicaklik_etkinlik
Java101_10 Hava sıcaklığına göre etkinlik öneren program

/* Ödev - Patika.dev
Aynı örnek üzerinden if koşulları başka hangi şekilde oluşturulabilirdi farklı çözüm yolları bulunuz.
Koşullar :

Sıcaklık 5'dan küçük ise "Kayak" yapmayı öner.
Sıcaklık 5 ve 15 arasında ise "Sinema" etkinliğini öner.
Sıcaklık 15 ve 25 arasında ise "Piknik" etkinliğini öner.
Sıcaklık 25'ten büyük ise "Yüzme" etkinliğini öner. */

import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
	    int heat ;
	    
	    Scanner input=new Scanner(System.in);
	    System.out.print("Hava sıcaklığı kaç derece ? ");
	    heat=input.nextInt();
	    
	    if (heat<5) {
	        System.out.print("Kayak havası !");
	    }
	    else if (heat>=5 && heat<10){
	        System.out.print("Sinema zamanı !");
	    }
	    else if (heat>=10 && heat<15){
	        System.out.print("Sinema ya da pikniğe gidebilirsin !");
	    }
	    else if (heat>15 && heat<=25){
	        System.out.print("Piknik zamanı !");
	    }
	    else {
	        System.out.print("Yüzme zamanı !");
	    }
		
	}
}
