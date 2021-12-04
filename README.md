# Terminal-Calculator
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner s =new Scanner (System.in);
	    
		System.out.println(" ---------------------|| TERMINAL CLACULATOR ||---------------------");
		
		System.out.println("");
		System.out.println("");
	
	 boolean n=true;
	 while(n==true)
	 {
	   	System.out.print("Enter the first number upon which you have to perform opertion : ") ;
		double a =s.nextDouble();
		
		System.out.print("Enter the Second number upon which you have to perform opertion : ") ;
		double b =s.nextDouble();
		
		
		
		System.out.println("");
		System.out.println("Select the number corresponding to the opeartion you want to perform : ");
		System.out.println("1. Addition 2.Substraction 3.Multiplication 4.Division");
		int choice = s.nextInt();
		System.out.println("");
	
		
		
		switch(choice)
		{
		  case 1 : 
		      double c = a+b;
		      System.out.println("Output : "+c);
		      break;
		  case 2 : 
		      double d=0;
		      if(a>b){d=a-b;}
		       d = b-a;
		      System.out.println("Output : "+d);
		      break;
		  case 3 : 
		      double e = a*b;
		      System.out.println("Output : "+e);
		      break;
		  case 4 : 
		      double f = a/b;
		      System.out.println("Output : "+f);
		      break;
		  default:
		      System.out.println("Invalid opeartion");
		}  
		
		System.out.println("Do you want to continue ? ");
		System.out.println("yes/no");
		
		String str = s.next();
		
		if(str=="yes" || str == "YES")
		{
		    n=false;
		}
		
	 }
	}
}
