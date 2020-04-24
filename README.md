# Java-Basic-1
Java Basic #1Function คำนวณค่าลงทะเบียนเรียน คิดเป็นราย ชม ต่อ คน ด้วย If Eles (โดยที่ยังไม่ได้checkค่าที่รับเข้ามา).
https://www.onlinegdb.com/online_java_compiler#

import java.util.Scanner;
import java.util.ArrayList;
public class Main
{
    
	public static void main(String[] args) {

      Scanner Keyboard = new Scanner(System.in);
      
		  System.out.print("Enter number of Student :" );
			int St1 = Keyboard.nextInt();
			System.out.print("Enter Hours :" );
			int Hours = Keyboard.nextInt();
      
			int[] total = new int[5];
			total[0]=500;
			total[1]=450;
			total[2]=400;
			total[3]=350;
			total[4]=300;
      
		if(St1 ==1 && Hours>=1){
		System.out.println("Student "+St1+" ("+total[0]+"฿ *"+Hours+"Hours ="+(total[0]*Hours)+"฿)");
		System.out.println("Student "+St1+" will paid about = "+(total[0]*Hours)*St1+"฿");
		  }else if(St1 ==2 && Hours>=1){
		System.out.println("Student "+St1+" ("+total[1]+"฿ *"+Hours+"Hours ="+(total[1]*Hours)+"฿)");
		System.out.println("Student "+St1+" will paid about = "+(total[1]*Hours)*St1+"฿");
		  }else if(St1 ==3 && Hours>=1){
		System.out.println("Student "+St1+" ("+total[2]+"฿ *"+Hours+"Hours ="+(total[2]*Hours)+"฿)");
		System.out.println("Student "+St1+" will paid about = "+(total[2]*Hours)*St1+"฿");
		  }else if(St1 ==4 && Hours>=1){
		System.out.println("Student "+St1+" ("+total[3]+"฿ *"+Hours+"Hours ="+(total[3]*Hours)+"฿)");
		System.out.println("Student "+St1+" will paid about = "+(total[3]*Hours)*St1+"฿");
		  }else{
		  System.out.println("Student "+St1+" ("+total[4]+"฿ *"+Hours+"Hours ="+(total[4]*Hours)+"฿)");
		  System.out.println("Student "+St1+" will paid about = "+(total[4]*Hours)*St1+"฿");
		  }      
	 }
}


/**   ผลลัพธิ์ **/

Enter number of Student :5                                                                       
Enter Hours :1                                                                                   
Student 5 (300฿ *1Hours =300฿)                                                                   
Student 5 will paid about = 1500฿ 



