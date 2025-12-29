This is my First Repository
Author - Vidhi Sontakke
import java.util.Scanner;
import java.util.Random;

class GuessGame {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        Random rand = new Random();

        int computerNumber = rand.nextInt(10) + 1;

        System.out.print("Guess a number between 1 to 10: ");
        int userGuess = sc.nextInt();

        if (userGuess == computerNumber) {
            System.out.println("🎉 You Win! Correct Guess");
        } else {
            System.out.println("❌ Wrong Guess");
            System.out.println("Computer number was: " + computerNumber);
        }
    }
}
