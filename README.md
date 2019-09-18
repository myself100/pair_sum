# pair_sum
package elclipse;
import java.util.*;
public class pairsum1 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int a[]= {2,8,5,7,6,1,9,5,3};

		int n=a.length;
		int sum=10;
		pairsum(a,n,sum);   //calling pairsum method
		
	
}
	public static void pairsum(int a[],int n,int sum) {
		
		for(int i=0;i<n;i++) {
			for(int j=i+1;j<n;j++) {
				if(a[i]+a[j]==sum) {    ///checking condition
					System.out.println(i + " " +j);
				}
			}
		}
	}
  
  
 ///time complexity is O(n^2);
