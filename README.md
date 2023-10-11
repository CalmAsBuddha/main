import java.util.Scanner;


public class Main {
    public static void main(String args[]) {
//        Scanner sc = new Scanner(System.in);
//        int size = sc.nextInt();
//        int numbers[] = new int[size];
//
//
//        for(int i=0; i<size; i++) {
//            numbers[i] = sc.nextInt();
//        }
//
//
//        //print the numbers in array
//        for(int i=0; i<arr.length; i++) {
//            System.out.print(numbers[i]+" ");
//        }

   Scanner sc = new Scanner(System.in);
   int row = sc.nextInt();
   int cols = sc.nextInt();
   int[][] number = new int[row][cols];


   //input
        for(int i = 0;i<row;i++){
            for (int j = 0 ; j < cols;j++){
                number[i][j] = sc.nextInt();
            }
        }



    //output
    for (int i =0;i < row;i++){
        for(int j = 0;j<cols;j++){
                System.out.print(number[i][j] + " ");
            }System.out.println();
        }
    //to find the number's location
        int x = sc.nextInt();


    for (int i = 0;i<row;i++){
        for(int j = 0;j<cols;j++){
            if (number[i][j] == x ) {
                System.out.println("The location of x is (" + i + ", " + j + ")");
            }

            }
        }


    }
}
