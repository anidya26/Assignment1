/*import java.util.*;
import java.io.*;
class Assignment1
{
    public static void main( String args[])
    {
        int num, sq,i,ext, sum=0;
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter a number");
        num=sc.nextInt();
        sq=num*num;
        while(sq>0)
        {
            ext=sq%10;
            sum = sum+ ext;
            sq=sq/10;
        }
        if ( sum == num)
        {
            System.out.println("Neon Number");
        }
        else
        {
            System.out.println("Not a neon number");
        }
        }
    }

    

import java.util.*;
import java.io.*;
//class Assignment1
{
    public static void main(String args[])
    {
        int i, dig=0,n, ext, temp, lastdig, sum = 0;
        Scanner sc= new Scanner(System.in);
        System.out.println("Enter a number");
        n=sc.nextInt();
        temp=n;
        while(temp>0)
        {
            temp = temp/10;
            dig++;
        }
        temp = n;
        for(i = n; i>0; i= i/10)
        {
            ext = temp%10;
            sum = sum + (int)Math.pow(ext,dig);
        }
        if(sum == n)
        System.out.println("It is an Armstrong Number");
        else
        System.out.println("Not an Armstrong number");
        }
    }
    
    
    
    
    
    
import java.util.*;
import java.io.*;
 class assignment1
{
   static boolean isValidISBN(String isbn)
    {
        int n = isbn.length();
        //if (n != 10)
            return false;
        int sum = 0;
        for (int i = 0; i < 9; i++)
        {
            int digit = isbn.charAt(i) - '0';
            if (0 > digit || 9 < digit)
                return false;
            sum += (digit * (10 - i));
        }
        char last = isbn.charAt(9);
        if (last != 'X' && (last < '0' ||
                            last > '9'))
            return false;
        sum += ((last == 'X') ? 10 : (last - '0'));
        return (sum % 11 == 0);
    }
    public static void main(String[] args)
    {
        String isbn = "007462542X";
        if (isValidISBN(isbn))
            System.out.print("Valid");
        else
            System.out.print("Invalid");
    }
}  */
