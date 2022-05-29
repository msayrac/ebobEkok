# ebobEkok
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int n1, n2;

        Scanner input = new Scanner(System.in);
        System.out.println("1. sayiyi giriniz : ");
        n1 = input.nextInt();

        System.out.println("2. sayiyi giriniz : ");
        n2 = input.nextInt();

        System.out.println("*******EBOB Hesabi**********");
        int ebob = 1;
        for (int i = 1; i <= n1; i++) {
            if (n1 % i == 0 && n2 % i == 0) {
                ebob = i;
            }
        }
        System.out.println(n1 + " ve " + n2 + " ebob " + "degeri : " + ebob);

        System.out.println("*******EKOK Hesabi**********");
        int ekok=1;

        for(int i=1; i<=(n1*n2);i++){
            if(i%n1==0 && i%n2==0){

                ekok=i;
                break;

            }
        }
        System.out.println(n1 + " ve " + n2 + " ekok " + "degeri : " + ekok);


    }
}
