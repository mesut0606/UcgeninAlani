ÇGENİN ALANINI HESAPLAMA import java.util.Scanner;

public class Main { public static void main(String[] args) { // Formül //Üç𝑔𝑒𝑛𝑖𝑛 ç𝑒𝑣𝑟𝑒𝑠𝑖 = 2𝑢 // //𝑢 = (a+b+c) / 2 // //Alan * Alan = 𝑢 * (𝑢 − 𝑎)* (𝑢 − 𝑏) * (𝑢 − 𝑐)

// Değişkenler
int a, b, c;
double u, alan;

// Kullanıcıdan veri alma

Scanner girdi = new Scanner(System.in);
System.out.print("1. Kenar Uzunluğunu Giriniz :");
a= girdi.nextInt();
System.out.print("2. Kenar Uzunluğunu Giriniz :");
b= girdi.nextInt();
System.out.print("3. Kenar Uzunluğunu Giriniz :");
c= girdi.nextInt();

u= (a+b+c) / 2;
System.out.println("Çevresi :" +2 * u);

alan = Math.sqrt (u * (u-a)* (u-b) * (u-c));

System.out.println("Alan : " +alan);
} }