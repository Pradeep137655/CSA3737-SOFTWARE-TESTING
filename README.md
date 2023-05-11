# CSA3737-SOFTWARE-TESTING

 1 Write a white box testing code ( junit ) to reverse a word and using assert statement for Proof the value 
 CODE :
 
 package pradeep;
import static org.junit.Assert.assertEquals;
import java.util.Scanner;
public class reverse {
	public static void main(String[] args)
	{
		String str; 
		char ch; 
		Scanner sc=new Scanner(System.in);
		System.out.print("Enter a string : "); 
		str=sc.nextLine();
		System.out.println("Reverse of a String '"+str+"' is :"); 
		for(int j=str.length();j>0;--j)
		{
			System.out.print(str.charAt(j-1));
		assertEquals("sse",str);
				} 
			assertEquals("sse",str);
			
	}

}

OUTPUT :

![Screenshot (97)](https://github.com/Pradeep137655/CSA3737-SOFTWARE-TESTING/assets/112744426/d9b111f9-6d38-4c64-a78b-0778e256cb1d)

2 Write a white box testing code ( junit ) to String comparison of word and using assert statement for Proof the value
CODE :
package pradeep;
import static org.junit.Assert.assertEquals;
import java.util.Scanner;
public class compare {
	public static void main(String [] args)
	{ 
		Scanner in=new Scanner(System.in); 
			System.out.println("enter the user name"); 
		String str1=in.nextLine(); 
		System.out.println("Reenter the user name");
		String str2=in.nextLine(); 
		assertEquals(str1,str2);
			}

}
OUTPUT :

![Screenshot (98)](https://github.com/Pradeep137655/CSA3737-SOFTWARE-TESTING/assets/112744426/afbcafc2-4b7e-4454-a12a-90625eb5bc2c)

3. Write a junit code for voting system and uses assert statement and verify the white box testing?
CODE :
package pradeep;
import static org.junit.Assert.assertTrue;
import java.util.Scanner;
public class compare {
	public static void main(String[] args) 
	{ 
	int age,shrt;
	Scanner scan = new Scanner(System.in);
	System.out.println(" Please enter your age");
	age = scan.nextInt(); 
	if(age>=18) 
	{ 
	System.out.println("Welcome to voting system Yo can Vote");
	} 
	else
	{
		shrt= (18 - age);
	System.out.println("Sorry,You can vote after :"+ shrt + " years");
	assertTrue(age==shrt);

	} }

}

OUTPUT :
![Screenshot (99)](https://github.com/Pradeep137655/CSA3737-SOFTWARE-TESTING/assets/112744426/4481a5dd-484e-4f74-a3f5-728412669daa)

4. Write a program using function to calculate the simple interest. Suppose the customer is a senior citizen. He is being offered 12 percent rate of interest; for all other customers, the ROI is 10 percent. The output values should verify using white box testing?
CODE :
package pradeep;
import static org.junit.Assert.assertTrue;
import java.util.Scanner;
public class compare {
	public static void main(String[] args)
	{ 
		Scanner sc=new Scanner(System.in);
		float P=sc.nextFloat(); 
		float R=sc.nextFloat(); 
		float T=sc.nextFloat(); 
		float SI = (P * T * R) / 100; 
		System.out.println("Simple interest = " + SI);
		assertTrue(3600==SI);
		}
}

OUTPUT :

![Screenshot (100)](https://github.com/Pradeep137655/CSA3737-SOFTWARE-TESTING/assets/112744426/f13f1d84-8115-4229-ad8e-ea3197a28477)

5. Given number is palindrome or not and verify The output values should verify using white box testing?
CODE :
package pradeep;
import java.util.Scanner;
import static org.junit.Assert.assertTrue;
public class compare {
	public static void main(String args[]) 
	{ 
		Scanner in = new Scanner(System.in);
		int r, sum = 0, temp; int n = in.nextInt();
		temp = n; 
		while (n > 0) 
		{
			r = n % 10; n = n / 10;
			sum = (sum * 10)+r;
		}
		System.out.println(sum);
		assertTrue(787==sum);
		if(temp==sum)
			System.out.println(sum+" is palindrome number");
		else
			System.out.println(sum+" is not palindrome number");
		} 
}

OUTPUT :
![Screenshot (101)](https://github.com/Pradeep137655/CSA3737-SOFTWARE-TESTING/assets/112744426/b5d86186-602b-486e-bece-74bf456270f4)

6. Write a program to convert Decimal number equivalent to Binary number and octal numbers? The output values should verify using white box testing?
CODE :
package pradeep;
import static org.junit.Assert.assertTrue;

import java.util.Scanner;
public class compare {

	public static void main(String[] args) 
	{ Scanner in = new Scanner(System.in); 
	// decimal number
	int decimal = in.nextInt(); 
	// convert decimal to binary
	String binary = Integer.toBinaryString(decimal); 
	
	System.out.println("BINARY IS " + binary); 
	//convert decimal to octal
	System.out.print("OCTAL IS "); 
	System.out.println(Integer.toOctalString(decimal));
	//assertEqual("1100" , binary);
	assertTrue(14== decimal);
	
	 }
}

OUTPUT :
![Screenshot (102)](https://github.com/Pradeep137655/CSA3737-SOFTWARE-TESTING/assets/112744426/6bad67c1-f45b-4d9c-b8de-34077ca954f0)

7. Write a Java Program to Convert a Given Number of Days in Terms of Years, Weeks & Days. The output values should verify using white box testing?
CODE :
package pradeep;
import static org.junit.Assert.assertTrue;
import java.util.Scanner;
public class compare {
	public static void main(String args[]) 
	{ 
		int m, year, week, day; 
		Scanner s = new Scanner(System.in);
		System.out.print("Enter the number of days:"); 
		m = s.nextInt(); 
		year = m / 365; 
		assertTrue(2==year);
		m = m % 365; 
		System.out.println("No. of years:"+year);
		week = m / 7;
		m = m % 7;
		System.out.println("No. of weeks:"+week); 
		day = m; 
		System.out.println("No. of days:"+day); } 
}

OUTPUT :
![Screenshot (103)](https://github.com/Pradeep137655/CSA3737-SOFTWARE-TESTING/assets/112744426/5514a8ab-db03-40cc-9971-4adfb9c69931)

8. Find the factorial of n? The output values should verify using white box testing?
CODE :
package pradeep;
import static org.junit.Assert.assertTrue;
import java.util.Scanner;
public class compare {
	public static void main(String[] args)
	{
	int i,j,pr=1;
	try{
	Scanner s=new Scanner(System.in);
	System.out.println("Enter the number to find the factorial");
	int n=s.nextInt();
	if(n<0)
	{
	System.out.println("Invalid");
	}
	else if(n==0)
	{
	System.out.println("1");
	}
	else
	{
	for(i=n;i>0;i--)
	{
	pr=pr*i;
	}
	System.out.println("The answer is:"+pr);
	assertTrue(120==pr);
	}
	}
	catch(Exception e)
	{
	System.out.println("Invalid");
	}
	}

}

OUTPUT :
![Screenshot (104)](https://github.com/Pradeep137655/CSA3737-SOFTWARE-TESTING/assets/112744426/a0a9d92b-3721-420a-b42e-bafe0b6efd63)

9. Find the year of the given date is leap year or not .The output values should verify using white box testing?
CODE :
package pradeep;
import static org.junit.Assert.assertTrue;
import java.util.Scanner;
public class compare {
	public static void main(String[] args)
	{
	int i=0;
	System.out.println("Enter the date/month/year");
	Scanner s=new Scanner(System.in);
	String re=s.next();
	String[] r=re.split("/",3);
	int x=Integer.parseInt(r[2]);
	assertTrue(x==2000);
	if(x%4==0)
	{
	System.out.println("It is an leap year");
	
	}
	else{
	System.out.println("It is not a leap year:");
	}
	}
}

OUTPUT :
![Screenshot (105)](https://github.com/Pradeep137655/CSA3737-SOFTWARE-TESTING/assets/112744426/472a7254-7d54-4e23-8036-9afffb8f3440)

10. Write a program to find the square, cube of the given decimal number. The output values should verify using white box testing?
CODE :
package pradeep;
import static org.junit.Assert.assertTrue;
import java.util.Scanner;
public class compare {
	public static void main(String[] args) 
	{ 
	try{ 
	Scanner s=new Scanner(System.in); 
	System.out.println("Enter an number"); 
	double n=s.nextDouble(); 
	double a=0,b=0; 
	a=n*n; 
	b=n*n*n; 
	System.out.println("The square of number="+a); 
	System.out.println("The square of number="+b); 
	} 
	catch(Exception e) 
	{ 
	System.out.println("Invalid"); 
	} 
	} 
	assertTrue(expected output==a);
	assertTrue(expected output ==b);
}

OUTPUT :
![Screenshot (106)](https://github.com/Pradeep137655/CSA3737-SOFTWARE-TESTING/assets/112744426/486d9ce4-9d49-4149-aefe-088139e118de)
