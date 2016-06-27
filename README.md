# PrimeCheckJava

import java.util.Scanner;

public class PrimeCheck 
{
	   private static Scanner scan;

	public static void main(String args[])
	   {		
		int temp;
		boolean isPrime=true;
		scan = new Scanner(System.in);
		System.out.println("Enter a number for check:");
		//capture the input in an integer
		int num=scan.nextInt();
		for(int i=2;i<=num/2;i++)
		{
	           temp=num%i;
		   if(temp==0)
		   {
		      isPrime=false;
		      break;
		   }
		}
		//If isPrime is true then the number is prime else not
		if(isPrime)
		   System.out.println(num + " is Prime Number");
		else
		   System.out.println(num + " is not Prime Number");
	   }
	}

Output 1
Enter a number for check:
7
7 is Prime Number

Output 2
Enter a number for check:
8
8 is not Prime Number
