# Upper-Array
Upper Array in java
import java.util.Scanner;

public class Upperarray {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the dimension of array:");
        int n = sc.nextInt();
        int[][] arr = new int[n][n];
        System.out.println("Enter the Elements of array");
        for(int i = 0;i<n;i++){
            for(int j = 0; j<n;j++){
            arr[i][j] = sc.nextInt();
            }
        }
        for(int i = 0; i< n; i++){
            for(int j = 0; j<n; j++){
                if (j>=i){
                System.out.print(arr[i][j]+" ");
                }else {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }

    }
}
