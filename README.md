# KDV Tutarı Hesaplayan Program
---
Bu bir [patika.dev](www.patika.dev) projesidir.
```
import java.util.Scanner;
public class kdvTutariHesaplama {
    public static void main(String[] args) {
        double kdvsizFiyat,kdvtutari,kdvliFiyat;
        Scanner input = new Scanner (System.in);
        System.out.print("Ürünün Fiyatını Giriniz:");
        kdvsizFiyat = input.nextInt();
        double kdvorani = kdvsizFiyat > 1000 ? 0.08 : 0.18;
        kdvtutari = kdvsizFiyat * kdvorani;
        kdvliFiyat = kdvsizFiyat + kdvtutari;

        System.out.println("KDV'siz Tutar:" +kdvsizFiyat);
        System.out.println("KDV Oranı:" +kdvorani);
        System.out.println("KDV Tutarı:" +kdvtutari);
        System.out.println("KDV'li Fiyat:" +kdvliFiyat);
    }
}
```
