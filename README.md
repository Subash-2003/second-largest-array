# second-largest-array
I have complted second largest array number in java.

import java.util.*;
public class Main
{
	public static void main(String[] args)
	{
	    Scanner sc = new Scanner(System.in);
	    int n = sc.nextInt();
	    int b=0,i,j;
	    int a[]=new int[n];
	    
    	for (i=0;i<n;i++)
    	    {
    	        a[i]=sc.nextInt();
    	    }
    	    
    	for (i=0;i<n;i++)
    	{
            for (j=i+1;j<n;j++)
            {
    	        if (a[i]>a[j])
    	        {
    	          b=a[j];
    	        }
    	        else  if (a[i] > b && a[i] != a[j])
    	        {
    	            b = a[i];
    	        }
            }
    	}
           System.out.println(b);
	}
}

