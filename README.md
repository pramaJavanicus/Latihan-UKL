# Latihan-UKL
import java.util.Scanner;

public class SoalMudah2 {

    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        System.out.print("Masukkan sebuah bilangan: ");
        int bilangan = scanner.nextInt(); 
        if (bilangan % 2 == 0) {
            System.out.println(bilangan + " adalah bilangan genap.");
        } else {
            System.out.println(bilangan + " adalah bilangan ganjil.");
        }
        scanner.close();
    }

}
import java.util.Scanner;

public class SoalMudah {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        20
        System.out.println("=== Program Menghitung Biaya Pengiriman ===");
        System.out.print("Masukkan panjang paket (cm): ");
        double panjang = scanner.nextDouble();
        System.out.print("Masukkan lebar paket (cm): ");
        double lebar = scanner.nextDouble();
        System.out.print("Masukkan tinggi paket (cm): ");
        double tinggi = scanner.nextDouble();
        System.out.print("Masukkan berat paket (kg): ");
        double berat = scanner.nextDouble();
        System.out.print("Masukkan jarak tempuh (km): ");
        double jarak = scanner.nextDouble();
        
        double volume = panjang * lebar * tinggi;
        double biayaBerat;
        if (jarak <= 10) {
            biayaBerat = berat * 4250;
        } else {
            biayaBerat = berat * 6000;
        }
        
        double biayaVolume = 0;
        if (volume > 100) {
            biayaVolume = 50000;
        }
        
        double totalBiaya = biayaBerat + biayaVolume;
        
        System.out.println("Volume paket: " + volume + " cm³");
        System.out.println("Biaya berat: Rp " + biayaBerat);
        System.out.println("Biaya volume: Rp " + biayaVolume);
        System.out.println("Total biaya pengiriman: Rp " + totalBiaya);
        
        scanner.close();
    }
}
