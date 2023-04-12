    import java.util.Scanner;

     public class artıkyıl {

      public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.print("Bir yil giriniz: ");
        int yil = input.nextInt();

        boolean artik = false;

        if (yil % 4 == 0) {
            if (yil % 100 == 0) {
                if (yil % 400 == 0) {
                    artik = true;
                }
            } else {
                artik = true;
            }
        }

        if (artik) {
            System.out.println(yil + " artik yildir.");
        } else {
            System.out.println(yil + " artik yil degildir.");
        }
    }

}
