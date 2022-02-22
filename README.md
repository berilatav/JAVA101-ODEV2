KDV Hesaplama

import java.util.Scanner;

public class KdvTutarHesaplama {
    public static void main(String[] args) {

        double tutar, kdvOran, kdvTutar ;
        Scanner input = new Scanner (System.in);
        System.out.println("Ücret tutarını giriniz: ");
        tutar = input.nextInt();

        if (tutar > 1000) {
            kdvOran = 0.18;
            kdvTutar = tutar * kdvOran;
            System.out.println("KDV Tutarınız: " + kdvTutar);
        }

        else {
            kdvOran = 0.08;
            kdvTutar = tutar * kdvOran;
            System.out.println("KDV Tutarınız: " + kdvTutar);
        }

    }
}

