# Repo-55
Program for Armstrong number
import java.util.*;
   public class Fifth {
    public static boolean isArmstrong(int num){
      int n = num;
      int cnt = String.valueOf (num).length();
      int sum = 0;
      while(n!=0){
         int rem = n % 10;
         sum += Math.pow(rem, cnt);
         n = n / 10;
      }
         return num == sum;
    }
    public static void main(String[] args)
    {
      Scanner sc = new Scanner(System.in);
      int num = sc.nextInt();
      if(isArmstrong(num)){
         System.out.println("yes its an armstrong number");
   }else {
      System.out.println("no");
   }
   sc.close();
}
   }
