# Exp2
```java
import java.util.Scanner; 
public class QuadraticEquation { 
    public static void main(String[] args) { 
        Scanner scanner = new Scanner(System.in); 
        System.out.print("Enter coefficient a: "); 
        double a = scanner.nextDouble(); 
        System.out.print("Enter coefficient b: "); 
        double b = scanner.nextDouble(); 
        System.out.print("Enter coefficient c: "); 
        double c = scanner.nextDouble(); 
        scanner.close(); 
        double discriminant = b * b - 4 * a * c; 
        if (discriminant > 0) { 
            double root1 = (-b + Math.sqrt(discriminant)) / (2 * a); 
            double root2 = (-b - Math.sqrt(discriminant)) / (2 * a); 
            System.out.println("The roots are real and distinct."); 
            System.out.println("Root 1: " + root1); 
            System.out.println("Root 2: " + root2); 
        } else if (discriminant == 0) { 
            double root = -b / (2 * a); 
            System.out.println("The root is real and equal."); 
            System.out.println("Root: " + root); 
        } else {
               double realPart = -b / (2 * a); 
            double imaginaryPart = Math.sqrt(-discriminant) / (2 * a); 
            System.out.println("The roots are complex and distinct."); 
            System.out.println("Root 1: " + realPart + " + " + imaginaryPart + "i"); 
            System.out.println("Root 2: " + realPart + " - " + imaginaryPart + "i"); 
        }
}
}
```
<img width="784" height="519" alt="Qudratic ouput" src="https://github.com/user-attachments/assets/d4d16c8b-b84b-460d-8a3c-3281b71147f9" />
