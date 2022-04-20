# Inheritance.
PBO D
package inheritance;

import java.util.Scanner;

public class main {
    public static void main(String[] args) {

        int pilih, pilihan;

        tradisional trd = new tradisional();
        modern mdn = new modern();
        gitar gtr = new gitar();
        drum drm = new drum();
        piano pno = new piano();
        kendang knd = new kendang();
        gangsa gns = new gangsa();
        gong gng = new gong();

        Scanner scan = new Scanner(System.in);

        System.out.println("program sederhana pemilihan alat musik");
        System.out.println("pilih jenis musik : ");
        System.out.println("=========================");
        System.out.println("modern = pilih 1");
        System.out.println("tradisional = pilih 2");
        System.out.println("pilih : ");
        pilih = scan.nextInt();

        if(pilih == 1){
            mdn.jenis();
            mdn.fungsimusik();
            System.out.println("pilih alat musik : ");
            System.out.println("===================");
            System.out.println("gitar = 1");
            System.out.println("drum = 2");
            System.out.println("piano = 3");
            System.out.println("masukan angka pilihan : ");
            pilihan = scan.nextInt();
            if(pilihan == 1){
                gtr.alat();
                gtr.bahan();
            }
            else if(pilihan == 2){
                drm.alat();
                drm.bahan();
            }
            else{
                pno.alat();
                pno.bahan();
            }
        }
        else{
            trd.jenis();
            trd.fungsimusik();
            System.out.println("pilih alat musik : ");
            System.out.println("===================");
            System.out.println("kendang = 1 ");
            System.out.println("gansa = 2 ");
            System.out.println("gong = 3 ");
            System.out.println("masukan angkah pilihan : ");
            pilihan = scan.nextInt();
            if(pilihan == 1){
                knd.alat();
                knd.bahan();
            }
            else if (pilihan == 2){
                gns.alat();
                gns.bahan();
            }
            else{
                gng.alat();
                gng.bahan();
            }
        }
    }
}
