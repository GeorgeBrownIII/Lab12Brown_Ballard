
package Lab12;

public class Lab12Prob01 {
	public static int recursiveAbstract(int n) {
        // Base cases
        if (n == 0) {
            return 1;
        } else if (n == 1) {
            return 3;
        } else if (n == 2) {
            return 4;
        }
        
        // Recursive case
        return recursiveAbstract(n - 3) * (recursiveAbstract(n - 2) - recursiveAbstract(n - 1));
    }
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		 System.out.println("f(0) = " + recursiveAbstract(0));  // Output: 1
	        System.out.println("f(1) = " + recursiveAbstract(1));  // Output: 3
	        System.out.println("f(2) = " + recursiveAbstract(2));  // Output: 4
	        System.out.println("f(3) = " + recursiveAbstract(3));  // Output: -1
	        System.out.println("f(4) = " + recursiveAbstract(4));  // Output: 15
	        System.out.println("f(5) = " + recursiveAbstract(5));  // Output: -64
	        System.out.println("f(6) = " + recursiveAbstract(6));  // Output: -79
	        System.out.println("f(7) = " + recursiveAbstract(7));  // Output: 225

	}

}