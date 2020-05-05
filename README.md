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

	int[] total = new int[6];
	total[0]=500;
	total[1]=450;
	total[2]=400;
	total[3]=350;
	total[4]=300;
	total[5]=0;

	if(St1 ==1 && Hours>=0){
	System.out.println("Student "+St1+" ("+total[0]+"฿ *"+Hours+"Hours ="+(total[0]*Hours)+"฿)");
	System.out.println("Student "+St1+" will paid about = "+(total[0]*Hours)*St1+"฿");
 	 }else if(St1 ==2 && Hours>=0){
	System.out.println("Student "+St1+" ("+total[1]+"฿ *"+Hours+"Hours ="+(total[1]*Hours)+"฿)");
	System.out.println("Student "+St1+" will paid about = "+(total[1]*Hours)*St1+"฿");
 	 }else if(St1 ==3 && Hours>=0){
	System.out.println("Student "+St1+" ("+total[2]+"฿ *"+Hours+"Hours ="+(total[2]*Hours)+"฿)");
	System.out.println("Student "+St1+" will paid about = "+(total[2]*Hours)*St1+"฿");
	  }else if(St1 ==4 && Hours>=0){
	System.out.println("Student "+St1+" ("+total[3]+"฿ *"+Hours+"Hours ="+(total[3]*Hours)+"฿)");
	System.out.println("Student "+St1+" will paid about = "+(total[3]*Hours)*St1+"฿");
 	 }else if(St1 ==0 && Hours==0){
 	 System.out.println("");
 	 System.out.println("Student "+St1+" ("+total[5]+"฿ *"+Hours+"Hours ="+(total[5]*Hours)+"฿)");
 	 System.out.println("Student "+St1+" will paid about = "+(total[5]*Hours)*St1+"฿");
	 }else{
	  System.out.println("Student "+St1+" ("+total[4]+"฿ *"+Hours+"Hours ="+(total[4]*Hours)+"฿)");
 	 System.out.println("Student "+St1+" will paid about = "+(total[4]*Hours)*St1+"฿");
 			 }        
		}
	}
 OR
  	
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
		
		int[] total = new int[6];
		total[0]=500;
		total[1]=450;
		total[2]=400;
		total[3]=350;
		total[4]=300;
		total[5]=total[5];
		
    switch (St1) {
      case 1:
	System.out.println("Student "+St1+" ("+total[0]+"฿ *"+Hours+"Hours ="+(total[0]*Hours)+"฿)");
	System.out.println("Student "+St1+" will paid about = "+(total[0]*Hours)*St1+"฿");
        break;
      case 2:
	System.out.println("Student "+St1+" ("+total[1]+"฿ *"+Hours+"Hours ="+(total[1]*Hours)+"฿)");
	System.out.println("Student "+St1+" will paid about = "+(total[1]*Hours)*St1+"฿");
        break;
     case 3:
	System.out.println("Student "+St1+" ("+total[2]+"฿ *"+Hours+"Hours ="+(total[2]*Hours)+"฿)");
	System.out.println("Student "+St1+" will paid about = "+(total[2]*Hours)*St1+"฿");
        break;
     case 4:
	System.out.println("Student "+St1+" ("+total[3]+"฿ *"+Hours+"Hours ="+(total[3]*Hours)+"฿)");
	System.out.println("Student "+St1+" will paid about = "+(total[3]*Hours)*St1+"฿");
        break;
     case 5:
	  System.out.println("Student "+St1+" ("+total[4]+"฿ *"+Hours+"Hours ="+(total[4]*Hours)+"฿)");
	  System.out.println("Student "+St1+" will paid about = "+(total[4]*Hours)*St1+"฿");
        break; 
     default:
	  System.out.println("Ohter Case");
	  System.out.println("Student "+St1+" ("+total[4]+"฿ *"+Hours+"Hours ="+(total[4]*Hours)+"฿)");
	  System.out.println("Student "+St1+" will paid about = "+(total[4]*Hours)*St1+"฿");
    }
        System.out.println();
        System.out.print("Enter Money:" );
        int MoneyIn = Keyboard.nextInt();
    	for(int i=0; i <=0; i++){
	    System.out.println("Exchange : "+(MoneyIn-(total[5]*Hours)*St1)+" ฿");
	}
   }
OR

	public class Main
	{
		public static void main(String[] args) {
	  	 
	    Scanner sc = new Scanner(System.in);
		System.out.print("Enter Student :");
			int student = sc.nextInt();  
		
		System.out.print("Enter Hours :");
		int hours = sc.nextInt();
		
		int[] total = new int[5];
		total[0]=500;
		total[1]=450;
		total[2]=400;
		total[3]=350;
		total[4]=300;
		
		int indexOfTotalStu = 0;
		int CaseOfStd = 0;
		int Calcu = 0;
		int ReciveMoney = 0;
		
		if(student >0)
		{
		    switch(student){
		      case 1 :
		    indexOfTotalStu = 0;
		    break;
		      case 2 :
		    indexOfTotalStu = 1;
		    break;
		      case 3 :
		    indexOfTotalStu = 2;
		    break;
		      case 4 :
		    indexOfTotalStu = 3;
		    break;
		    default :
		    indexOfTotalStu = 4;
		     break;
		    }
		int calcu = total[indexOfTotalStu]*hours;
	    System.out.println("Amout: "+calcu+ "฿");
	    
	    int Totalcal = calcu*student;
	    System.out.println("Amout for paid : "+Totalcal+ "฿");
		 
	    System.out.print("Enter Money:");
		int MoneyIn = sc.nextInt();
		
		ReciveMoney = MoneyIn-calcu;
	    System.out.print("Exchange : " +ReciveMoney+ "฿");
		    
		}
		else 
		{
		    	System.out.println("Can't calculate becase out of Enter student or Hours.");
		}
	
		}
	}

/**   ผลลัพธิ์ **/

	Enter number of Student :5                                                                       
	Enter Hours :1                                                                                   
	Student 5 (300฿ *1Hours =300฿)                                                                   
	Student 5 will paid about = 1500฿ 




HomeWork#23-04-2020 
Credit: http://www.comscicafe.com/article/105/java-basic-exercises-1#.XqKhs8gza03
ข้อที่ 1)
จงเขียนโปรแกรมด้วยภาษา Java ให้แสดงผลออกทางจอภาพตามตัวอย่าง
    
    Hello !
    Java Programming

ข้อที่ 2)
จงเขียนโปรแกรมด้วยภาษา Java ให้แสดงผลออกทางจอภาพตามตัวอย่าง (ต้องเว้นบรรทัดและเคาะวรรคตามตัวอย่าง)
    
    A B C
    ABC
    A A A
 
ข้อที่ 3)
จงเขียนโปรแกรมด้วยภาษา Java ทำการเก็บค่า 2 , 3 , 45 , 60 ,1500 และ ให้แสดงผลออกทางจอภาพตามตัวอย่าง (ต้องเว้นบรรทัดและเคาะวรรคตามตัวอย่าง)
 
    2 3 45
    60 1500
 
ข้อที่ 4)
จงเขียนโปรแกรมด้วยภาษา Java ทำการเก็บค่า 1 , 2 , 3 , 4 , 5 และ ให้แสดงผลออกทางจอภาพตามตัวอย่าง (ต้องเว้นบรรทัดและเคาะวรรคตามตัวอย่าง)
    
    1 2 3
    4 5 1
    2 3 4

ข้อที่ 5)
จงเขียนโปรแกรมด้วยภาษา Java ทำการเก็บค่า 1 , 2 , 3 , 4 , 5 และ ให้แสดงผลออกทางจอภาพตามตัวอย่าง (ต้องเว้นบรรทัดและเคาะวรรคตามตัวอย่าง)
    
    1 2 3 4 5
    54321

ข้อที่ 6)
จงเขียนโปรแกรมด้วยภาษา Java ทำการเก็บค่า 1 , 2 , 3 , 4 , 5 และ ให้แสดงผลออกทางจอภาพตามตัวอย่าง (ต้องเว้นบรรทัดและเคาะวรรคตามตัวอย่าง)
    
    1A2
    B21
    1 2 9
 
ข้อที่ 7)
จงเขียนโปรแกรมด้วยภาษา Java ทำการเก็บค่า H , e , l , o และ ให้นำค่าในตัวแปรมาแสดงผลออกทางจอภาพตามตัวอย่าง (ต้องเว้นบรรทัดและเคาะวรรคตามตัวอย่าง)
    
    Hello
    H
    e
    l
    l
    0


ข้อที่ 8)
จงเขียนโปรแกรมด้วยภาษา Java ทำการเก็บค่า 1 , 1.9 , A และ ให้นำค่าในตัวแปรมาแสดงผลแสดงผลออกทางจอภาพตามตัวอย่าง (ต้องเว้นบรรทัดและเคาะวรรคตามตัวอย่าง)

    1 , 1.9, A
    A1A
    1.91


ข้อที่ 9)
จงเขียนโปรแกรมด้วยภาษา Java ทำการเก็บค่า 1 , 2 , 3 และ ให้นำค่าในตัวแปรแสดงผลออกทางจอภาพตามตัวอย่าง (ต้องเว้นบรรทัดและเคาะวรรคตามตัวอย่าง)
    
    Enter Number : 1
    Enter Number : 2
    1 + 2 = 3
    1 + 1 = 2
    3 - 2 = 1
    2 - 1 = 1

ข้อที่ 10)
จงเขียนโปรแกรมด้วยภาษา Java ทำการเก็บค่า 1 , 2 , 3 , A , B  และ ให้นำค่าในตัวแปรแสดงผลออกทางจอภาพตามตัวอย่าง (ต้องเว้นบรรทัดและเคาะวรรคตามตัวอย่าง)

    Enter Number A : 1
    Enter Number B : 2
    A + B : 1 + 2 = 3
    A + A : 1 + 1 = 2
    (B - A) : 2 - 1 = 1
    (A + B) - 2 : (1 + 2) - 2 = 1


#เฉลย Function ไม่มีอะไรที่ตายตัวสามารถเปลี่ยนไปตามความคิดและความถนัดนะ อาจจะเขียนให้สั้นกว่านี้ได้ยิ่งดีค่ะ

import java.util.Scanner;
import java.util.ArrayList;

/** #1**/
    System.out.println ("------#1---------");
    
    System.out.println ("Hello! \nJava Programming");

/** #2**/
    System.out.println ("------#2---------");
    
    System.out.println ("A B C \nABC \nAAA");

/** #3**/
    System.out.println ("------#3---------");
    
    int[] i = new int[]{ 2, 3, 45, 60, 1500 };
      System.out.print (i[0] + " ");
      System.out.print (i[1] + " ");
      System.out.println (i[2]);
      System.out.print (i[3] + " ");
      System.out.println (i[4]);

/** #4**/
      System.out.println ("------#4---------");
    
    int[] number = new int[5];
      number[0] = 1;
      number[1] = 2;
      number[2] = 3;
      number[3] = 4;
      number[4] = 5;
    for (int o = 0; o < number[2]; o++)
      {
	System.out.print (number[o] + " ");
      }
    System.out.println ();
    for (int w = 3; w <= number[3]; w++)
      {
	System.out.print (number[w] + " ");
      }
    for (int o = 0; o < number[0]; o++)
      {
	System.out.print (number[o] + " ");
      }
    System.out.println ();
    for (int w = 1; w < number[3]; w++)
      {
	System.out.print (number[w] + " ");
      }
    System.out.println ();
    
/** #5**/
   System.out.println ("------#5---------");
    
    int[] num = new int[5];
    num[0] = 1;
    num[1] = 2;
    num[2] = 3;
    num[3] = 4;
    num[4] = 5;
    for (int e = 0; e < num.length; e++)
      {
	System.out.print (num[e] + " ");
      }
    System.out.println ();
    for (int z = 5; z >= 1; z--)
      {
	System.out.print (z);
      }

/** #6**/
    System.out.println ("------#6---------");
    
    ArrayList < String > TT = new ArrayList < String > ();
    TT.add ("1");
    TT.add ("A");
    TT.add ("2");
    for (int o = 0; o < TT.size (); o++){
	System.out.print (TT.get (o));
      }
	 System.out.println();
    ArrayList < String > TT2 = new ArrayList < String > ();
    TT2.add ("B");
    TT2.add ("2");
    TT2.add ("1");
    for (int e = 0; e < TT2.size (); e++) {
	System.out.print (TT2.get (e));
      }
    System.out.println ();
    ArrayList < String > TT3 = new ArrayList < String > ();
    TT3.add ("1 ");
    TT3.add ("2 ");
    TT3.add ("9 ");
    for (int c = 0; c < TT3.size (); c++){
          System.out.print (TT3.get (c));
      }
/** #7**/
    System.out.println ("------#7---------");
    
    String[]St = new String[4];
    St[0] = "H";
    St[1] = "e";
    St[2] = "l";
    St[3] = "o";
    System.out.println (St[0]+St[1]+St[2]+St[2]+St[3]);
    System.out.println (St[0]+"\n"+St[1]+"\n"+St[2]+"\n"+St[2]+"\n"+St[3]);
/** #8**/ 
 System.out.println ("------#8---------");
    
    int A = 1;
	float AB = 1.9f;
	String R = "A";
	 System.out.println(A+","+AB+","+R);
	 System.out.println(R+A+R);
	 System.out.println(AB+""+(A));

/** #9**/
    System.out.println ("------#9---------");
    
    Scanner Keyboard = new Scanner(System.in);
    System.out.print("Enter Number :");
     int t1 = Keyboard.nextInt();
    System.out.print("Enter Number :");
     int t2 = Keyboard.nextInt();
     System.out.println(t1 + " + " + t2 + " = " + (t1 + t2));
     System.out.println(t1 + " + " + t1 + " = " + (t1 + t1));
     System.out.println((t1 + t2) + " - " + (t1 + t1) + " = " + ((t1 + t2) - (t1 + t1)));
     System.out.println((t1 + t1) + " - " +((t1 + t2) - (t1 + t1)) + " = " +((t1 + t2) - (t1 + t1)));
  
    
/** #10**/
    System.out.println ("------#10---------");
  
    Scanner Keyboard = new Scanner(System.in);
    System.out.print("Enter Number A :");
     int t1 = Keyboard.nextInt();
    System.out.print("Enter Number B :");
     int t2 = Keyboard.nextInt();
     System.out.println("A+B:" + t1 + " + " + t2 + " = " + (t1 + t2));
     System.out.println("A+A:" + t1 + " + " + t1 + " = " + (t1 + t1));
     System.out.println("(B-A):" + (t1 + t1) + " - " + t1 + " = " + ((t1 + t1) - t1));
     System.out.println("(A+B)-2 :" + "(" + t1 + " + " + t2 + ")" + "-" + t2 + " = " + ((t1 + t2) - t2));
