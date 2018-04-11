# Nini
public class Antonini {

	public static void main(String[] args) {

		Scanner reader = new Scanner(System.in);
		System.out.println("Enter a number");
		int numberToCheck = reader.nextInt();
		reader.close();
		int firstNumber = 0, secondNumber = 1, fibonacciNumber = 0;
		while (fibonacciNumber < numberToCheck)
    {
			fibonacciNumber = firstNumber + secondNumber;
			firstNumber = secondNumber;
			secondNumber = fibonacciNumber;
		}
		
		if (numberToCheck == fibonacciNumber)
    {
			System.out.println("Числото е част от реда на Fibonacci");
		} else {
			System.out.println("Числото не е част от реда на Fibonacci");
		}
	}
}
