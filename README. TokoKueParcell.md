# UTS-Pemrograman-Mobile-2
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.tokokueparcell;

/**
 *
 * @author user
 */
import java.util.Scanner;

public class Tokokueparcell {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        // Pilih kue
        System.out.println("Selamat datang di Toko Kue Hampers Rijal Akmaludin!");
        System.out.print("Masukkan nama kue: ");
        String namaKue = input.nextLine();
        System.out.print("Masukkan harga kue: ");
        double hargaKue = input.nextDouble();
        input.nextLine(); // bersihkan newline

        Kue kue = new Kue(namaKue, hargaKue);

        // Data pelanggan
        System.out.print("Masukkan nama pelanggan: ");
        String namaPelanggan = input.nextLine();
        System.out.print("Masukkan alamat pengiriman: ");
        String alamat = input.nextLine();

        Pelanggan pelanggan = new Pelanggan(namaPelanggan, alamat);

        // Jumlah
        System.out.print("Masukkan jumlah yang dipesan: ");
        int jumlah = input.nextInt();

        // Buat pesanan
        Pesanan pesanan = new Pesanan(kue, pelanggan, jumlah);

        // Tampilkan rincian
        pesanan.tampilkanPesanan();
    }
}

