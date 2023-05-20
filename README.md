# Navintelusko
Assignment related pascale triangle

1. Iteration method 
public class PascalTriangle {
    public static void main(String[] args) {
        int numRows = 5;
        generatePascalTriangle(numRows);
    }
  
    public static void generatePascalTriangle(int numRows) {
        int[][] triangle = new int[numRows][];
        for (int i = 0; i < numRows; i++) {
            triangle[i] = new int[i + 1];
            triangle[i][0] = 1; // First element in each row is always 1
            triangle[i][i] = 1; // Last element in each row is always 1
            for (int j = 1; j < i; j++) {
                triangle[i][j] = triangle[i - 1][j - 1] + triangle[i - 1][j];
            }
        }
        // Print the Pascal's triangle
        for (int i = 0; i < numRows; i++) {
            for (int j = 0; j <= i; j++) {
                System.out.print(triangle[i][j] + " ");
            }
            System.out.println();
        }
    }
}
            
2.factorial method 

   public class PascalTriangle {
    public static void main(String[] args) {
        int numRows = 5;
        generatePascalTriangle(numRows);
    }
  
    public static void generatePascalTriangle(int numRows) {
        for (int i = 0; i < numRows; i++) {
            for (int j = 0; j <= i; j++) {
                int coefficient = calculateCoefficient(i, j);
                System.out.print(coefficient + " ");
            }
            System.out.println();
        }
    }
  
    public static int calculateCoefficient(int n, int k) {
        return factorial(n) / (factorial(k) * factorial(n - k));
    }
  
    public static int factorial(int num) {
        if (num == 0 || num == 1) {
            return 1;
        }
        int result = 1;
        for (int i = 2; i <= num; i++) {
            result *= i;
        }
        return result;
    }
}
    
3.fibonacci method 

public class PascalTriangle {
    public static void main(String[] args) {
        int numRows = 5;
        generatePascalTriangle(numRows);
    }
  
public class PascalTriangle {
    public static void main(String[] args) {
        int numRows = 5;
        generatePascalTriangle(numRows);
    }
  
    public static void generatePascalTriangle(int numRows) {
        for (int i = 0; i < numRows; i++) {
            for (int j = 0; j <= i; j++) {
                int coefficient = calculateCoefficient(i, j);
                System.out.print(coefficient + " ");
            }
            System.out.println();
        }
    }
  
    public static int calculateCoefficient(int n, int k) {
        return factorial(n) / (factorial(k) * factorial(n - k));
    }
  
    public static int factorial(int num) {
        if (num == 0 || num == 1) {
            return 1;
        }
        int result = 1;
        for (int i = 2; i <= num; i++) {
            result *= i;
        }
        return result;
    }
}

    



 

     

    

  

     
          

       
