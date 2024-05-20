import java.util.Scanner;

public class Main1 {
    public static void main(String[] args) {
    
        //kullanıcıdan alınan para değerinin kdvli fiyatını ve kdv tutarını hesaplayıp ekrana bastıran programı yaz
        // kdv tutarı %18   kdvsiz fiyat=10    kdvli fiyat=11.8  kdv tutarı=1.8

        
       double para,kdvOran=0.18;
       
        Scanner fiyat = new Scanner(System.in);
        System.out.print("Bir para değeri girin:  ");
        para = fiyat.nextDouble();
        
        double kdvTutar=para*kdvOran;
        double kdvliTutar=para+kdvTutar;
        
        System.out.println("KDVli Tutar: "+kdvliTutar);
        System.out.println("KDV Oran: "+kdvOran);
        



    }
}
