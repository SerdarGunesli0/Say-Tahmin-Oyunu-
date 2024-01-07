    import java.util.Scanner;
    import java.util.Random;

    public class Main {
        public static void main(String[] args) {
            final String ANSI_GREEN = "\u001B[32m";
            final String ANSI_RED = "\u001B[31m";
            Scanner scanner1 = new Scanner(System.in);
            System.out.print("Oyunu Başlatmak İçin: (Start) Programı Kapatmak İçin: (Quit) ");
            String soru1 = scanner1.nextLine();
            int anahtar_değeri = 1;

            if (soru1.equals("Quit")) {
                System.out.print("Program Kapatılıyor:");
                anahtar_değeri = 0;
            }

            if (soru1.equals("Start")) {
                Random rastgele_sayi_olusturu = new Random();
                int sayi_uretici = rastgele_sayi_olusturu.nextInt(35);
                System.out.print("O Halde Başlayalım Sayımız 0 ile 35 Arasında Olacak: ");
                int deneme_sayisi = 0;

                while (anahtar_değeri == 1) {
                    Scanner scanner2 = new Scanner(System.in);
                    int soru2 = scanner2.nextInt();
                    deneme_sayisi++;

                    if (soru2 == sayi_uretici) {
                        System.out.print("TEBRİKLER DOĞRU TAHMİN! Toplam " + deneme_sayisi + " Denemede Buldun Güzel :)\n");
                        anahtar_değeri = 0;
                    } else if (sayi_uretici > soru2) {
                        System.out.print("Daha Büyük Bir Sayı Mı Girsen Acaba? : ");
                    } else if (sayi_uretici < soru2) {
                        System.out.print("Biraz Uçtun Sanki He? Biraz Daha Düşük Rakamlar Canım Benim: ");
                    }

                    if (deneme_sayisi == 0) {
                        System.out.print("KARDEŞİM SEN NESİN BÖYLE TEK ATTIN ");
                        System.out.print("Aldığın Puan 100 " + ANSI_GREEN);
                    } else if (deneme_sayisi >= 3 && deneme_sayisi <= 5) {
                        System.out.print("ADAMMMMMM GÜZELDİN ALDIĞIN PUAN 85, Toplam " + deneme_sayisi + " Denemede Buldun\n");
                    } else if (deneme_sayisi >= 6 && deneme_sayisi <= 9) {
                        System.out.print("berbattın knk aldığın puan 50 " + deneme_sayisi + " Denemede Buldun\n");
                    } else if (deneme_sayisi >= 10) {
                        System.out.print("KÖR SENDEN DAHA İYİ YAPARDI KANKA" + deneme_sayisi + " Denemede Buldun\n");
                    }
                }
            } else {
                System.out.print("Geçerli Bir İşlem Giriniz :");
            }
        }
    }
