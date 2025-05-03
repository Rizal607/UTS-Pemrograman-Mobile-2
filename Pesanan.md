/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package com.mycompany.tokokueparcell;

/**
 *
 * @author user
 */
public class Pesanan {
    private Kue kue;
    private Pelanggan Pelanggan;
    private int jumlah;

    public Pesanan(Kue kue, Pelanggan pelanggan, int jumlah) {
        this.kue = kue;
        this.Pelanggan = pelanggan;
        this.jumlah = jumlah;
    }

    public void tampilkanPesanan() {
        System.out.println("=== Rincian Pesanan ===");
        System.out.println("Nama Pelanggan: " + Pelanggan.getNama());
        System.out.println("Alamat Pengiriman: " + Pelanggan.getAlamat());
        System.out.println("Kue: " + kue.getNama());
        System.out.println("Harga per item: " + kue.getHarga());
        System.out.println("Jumlah: " + jumlah);
        System.out.println("Total: Rp" + (kue.getHarga() * jumlah));
    }
}

