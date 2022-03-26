# KdvTutari
package com.company;

    import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        double tutar,kdv,kdvliTutar,kdvTutar;
        Scanner input=new Scanner(System.in);
        System.out.print("Ücret Tutarını Giriniz:");
        tutar=input.nextDouble();
        kdv=(tutar<=1000  ? 0.18 : 0.08) ;
        kdvTutar=tutar * kdv;
        System.out.println("Kdv Tutarı:" + kdvTutar);
        kdvliTutar=tutar+kdvTutar;
        System.out.println("KDV'li Tutar:" + kdvliTutar);
        System.out.println("KDV'siz Tutar:" + tutar);
        System.out.println("KDV Oranı:" + kdv);

    }
}
