import java.util.Scanner;

public class array {

	public static void main(String[] args) {
		Scanner sc=new Scanner(System.in);
		System.out.println("enter the rows");
		int n=sc.nextInt();
		System.out.println("enter the columns");
		int m=sc.nextInt();
		int[][] a=new int[n][m];
		for(int i=0;i<n;i++) {
			for(int j=0;j<m;j++) {
				a[i][j]=sc.nextInt();
			}
		}
		System.out.println("elements are");
		for(int i=0;i<n;i++) {
			for(int j=0;j<m;j++) {
				System.out.println(a[i][j]);
			}
		}
	}
}
