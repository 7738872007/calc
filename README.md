# calc
simple calculator
import java.util.*;
class calc
{
	public static void add(int a,int b)
	{
		System.out.println("a+b = "+(a+b));
	}
	
	public static void sub(int a,int b)
	{
		System.out.println("a-b = "+(a-b));
	}	
	
	public static void mul(int a,int b)
	{
		System.out.println("a*b = "+(a*b));
	}
	
	public static void div(int a,int b)
	{
		if(b==0)
			System.out.println("division not possible");
		else 
			System.out.println("a/b = "+(a/b));
		
	}
	
	public static void main(String args[])
	{
		Scanner src=new Scanner(System.in);
		int ch,x,y;
		do
		{
			System.out.println("enter a choice");
			System.out.println("1:Add 2:Sub 3:mul 4:Div 5:exit");
			ch=src.nextInt();
			
			
			switch(ch)
			{
				case 1:System.out.println("enter the two numbers");
			           x=src.nextInt();
			           y=src.nextInt();
				       add(x,y);
				       break;
				case 2:System.out.println("enter the two numbers");
			           x=src.nextInt();
			           y=src.nextInt();
				       sub(x,y);
            		   break;
				case 3:System.out.println("enter the two numbers");
			           x=src.nextInt();
			           y=src.nextInt();
				       mul(x,y);
 				       break;
				case 4:System.out.println("enter the two numbers");
			           x=src.nextInt();
			           y=src.nextInt();
				       div(x,y);
				       break;
				case 5:break;
			}
		}
		while(ch!=5);
	}
	
}
