# ArmStrong_Number
An Armstrong number of three digits is an integer such that the sum of the cubes of its digits is equal to the number itself.
//This is Written in My Favorite Language "Java";

import java.util.Scanner;
class ArmStrong_Number{
    public static void main(String[] args){
    Scanner sc = new Scanner(System.in);
int num = sc.nextInt();
   int t1 = num;
   int length = 0;
   while(t1>0){
	   length = length +1;
	   t1 = t1/10;
   }
   System.out.println(length);
   int t2 = num;
   int arm =0;
   int rem;
   while(t2>0){
	   rem = t2%10;
	   int mul = 1;
	   for(int i = 1; i<=length;i++){
          mul  = rem*mul;
	   }
	   arm = arm+mul;
	   t2 = t2/10;
   }
   System.out.println(arm);	

	}
}
