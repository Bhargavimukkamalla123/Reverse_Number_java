import java.util.Scanner;
public class ReverseNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter a number:");
        int num = sc.nextInt();
        int reverse = 0;
        while(num != 0) {
            int lastDigit = num % 10;
            reverse = reverse * 10 + lastDigit;
            num = num / 10;
            
        }
        System.out.println("Reversed number:" + reverse);
    }
}
