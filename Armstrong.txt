import java.util.Scanner;
import java.lang.Math;
public class Armstrong
{
   public static void main(String[] args)
    {
      Scanner sc = new Scanner(System.in);
      int n, count = 0, sum=0, last;
      System.out.println("Enter number: ");
      n = sc.nextInt();
      int num;
      num = n;
     while(num!=0)
    {
      count++;
      num=num/10;
    }
      while(n>0)
    {
        last = n%10;
        sum+=Math.pow(last,count);
        n = n/10;
    }
System.out.println(sum);
    if(sum==n)
    {
     System.out.println("Number is armstrong.");
     }
     else
{  
System.out.println("Number is not armstrong.");
}
}
}