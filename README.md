# javayla-kombinasyon-hesaplayan-program
System.out.println(y);

    import java.util.Scanner;

    public class Main {

    public static void main(String[] args) {

        int n, nFaktoru = 1, rFaktoru = 1, x, y = 1;
        double sonuc;
        Scanner inp = new Scanner(System.in);
        System.out.print(" n Sayısını Giriniz :");
        n = inp.nextInt();

        for (int i = 1; i <= n; i++) {

            nFaktoru *= i;
        }
        System.out.println(n + ". Faktöriyel :" + nFaktoru);
        System.out.print("-------------\n r Sayısını Giriniz :");

        int r = inp.nextInt();
        for (int a = 1; a <= r; a++) {
            rFaktoru *= a;

        }
        System.out.println(r + ".Faktöriyel :" + rFaktoru);

        x = n - r;
        for (int p = 1; p <= x; p++) {
            y *= p;
        }

        sonuc = (rFaktoru * (y)) / nFaktoru;
        System.out.println("C(n,r) :" + sonuc);

     }
    }





