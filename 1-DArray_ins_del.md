import java.util.*;
class Arrayinsertion {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("enter the elements");
        int n=sc.nextInt();
        int[] a=new int[n];
        int[] b=new int[n-1];
        for(int i=0;i<n;i++){
            a[i]=sc.nextInt();
        }
        System.out.println("delete elements");
        int m=sc.nextInt();
        for(int i=0;i<a.length;i++){
            if(i<m){
                b[i]=a[i];
            }else if(i==m){
                continue;
            }else{
                b[i-1]=a[i];
            }
        }
        System.out.println("enter the elements");
        for(int i=0;i<n-1;i++){
            System.out.println(b[i]);
        }
    }
}
