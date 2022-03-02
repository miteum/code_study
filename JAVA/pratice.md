

## 정올 실습 



![](C:/Users/%EC%9D%B4%EB%AF%BF%EC%9D%8C/OneDrive/%EB%B0%94%ED%83%95%20%ED%99%94%EB%A9%B4/%EC%9E%90%EA%B0%80%EC%A7%84%EB%8B%A8.jpg)



문제 풀기 



``` 
public static void main(java.lang.String[] args) {
		
		//출력 - 자가진단 1 
		System.out.println("Fun Programming!");
		
		//출력 - 자가진단 2
		System.out.println("Programming! It's fun. ");

		//출력 - 자가진단 3
		System.out.println("My name is Hong Gil Dong.");
		System.out.println("I am 13 years old.");
		
		//출력 - 자가진단 4
		System.out.println("(@)(@)\n(=^.^=_)\n(-m-m)");
		
		
		//출력 - 자가진단 5 
		System.out.printf("I can %s well.","program");
		System.out.printf("Dreams %s true.","come");
		
	}
	
```

```
//출력 - 자가진단 6
		int n = 170;
		double z = 68.6;
		
		System.out.printf("My height" + n + "My weight" + z); // 첫번째 방법
		
		System.out.printf("My height\n");
		System.out.printf("%d\n",n);
		System.out.printf("My weight\n");
		System.out.printf("%.6f",z);
		
		
		//출력 - 자가진단 7
		System.out.printf("5 Dan");
		System.out.printf("5 * 2 = 10");

		
		
		//출력 - 자가진단 8
		System.out.println("item  count  price");
		System.out.printf("pen, 20, 100\n");
		System.out.printf("note, 5, 95\n");
		System.out.printf("eraser, 110, 97\n");
```

---





``` 
	
		System.out.println("My name is Hong");
		
		
		//형성평가2
		System.out.println("My hometown");
		System.out.println("Flowering Mountain");
		
		
		//형성평가3
		System.out.printf("TTTTTTTTTT\n");
		System.out.printf("TTTTTTTTTT\n");
		System.out.printf("%5s\n","TT");
		System.out.printf("%5s\n","TT");
		System.out.printf("%5s\n","TT");
		
		
		//형성평가4
		int kor = 90;
		int mat = 80;
		int eng = 100;
		
		System.out.println("sum =" + "kor + mat + eng" );
		System.out.println(kor + mat + eng);
		
		
		
		//형성평가 5
	
  System.out.printf("%15s%15s%15s\n", "Seoul", "10,312,545", "+91,375");
  System.out.printf("%15s%15s%15s\n", "Pusan", "3,567,910", "+5,868");
  System.out.printf("%15s%15s%15s\n", "Incheon", "2,758,296", "+64,888");
  System.out.printf("%15s%15s%15s\n", "Daegu", "2,511,676", "+17,230");
  System.out.printf("%15s%15s%15s", "Gwangju", "1,454,636", "+29,774");

```



# 입력



```
		//입력 자가진단1 
		//정수형 변수를 선언하고 -100을 대입하여 출력하는 프로그램을 작성하라. 
		
		int i = -100; 
		System.out.println(i);
		
		
		//자가진단2
		//정수형 변수 2개를 선언하여 -1과 100을 대입한 후 아래와 같이 출력하는 프로그램을 작성하라.
		
		int j = -1;
		int z = 100; 
		System.out.println(j);
		System.out.println(z);
		
		
		
		//자가진단 3
		//두 개의 정수형 변수를 선언하고 값을 대입하여 아래와 같이 출력되는 프로그램을 작성하라.
		
		int a = 55;
		int b = 10; 
		
		System.out.println(a+"-"+b+"="+(a-b));
		
		int c = 2008;
		int d = 1999;
		
		System.out.println(c+"-"+d+"="+(c-d));
		
		
		
		/* 자가진단 4 추의 무게를 저장할 변수와 중력의 비율을 저장할 변수를 선언하고, 
		 * 다음 두 값을 변수에 저장하여 곱셈 계산식을 출력하는 프로그램을 작성하라. 
		 * 추의 무게 = 49, 중력의 비율 = 0.2683 */
		
		int w = 49;
		double x = 0.2683;
		
		System.out.println(w+"*"+x+"="+(w*x));
		
		
		//자가진단 5  
		//1야드(yd)는 91.44cm이고 1인치(in)는 2.54cm이다. 
		//2.1야드와 10.5인치를 각각 cm로 변환하여 다음 형식에 맞추어 소수 첫째자리까지 출력하시오.

		float yd = 91.44f;
		float in = 2.54f;
		
		System.out.printf("%4.1fyd = %5.1fcm\n", 2.1,2.1*yd);
		System.out.printf("%4.1fyd = %5.1fcm\n", 10.5,10.5*in);
		
	}

public class Main {
 public static void main(String[] args) {
  int a = -100;
  System.out.println(a);
 }
}



//정올 511 

	int a = 55;

		int b = 10;

		System.out.println(a + " - " + b + " = " + (a - b));

		a = 2008;

		b = 1999;

		System.out.println(a + " - " + b + " = " + (a - b));


////자가진단 4
		//추의 무게를 저장할 변수와 중력의 비율을 저장할 변수를 선언하고,다음 두 값을 변수에 저장하여 곱셈 계산식을 출력하는 프로그램을 작성하라.
		//추의 무게 = 49, 중력의 비율 = 0.2683
		
		int n = 49;
		double m = 0.2683;
			
		System.out.println(n * m);
		
		
		
		
		//자가진단6 
		
		키를 입력받아 출력하는 프로그램을 작성하라.
		(입력할때 "height = " 문장을 먼저 출력하고 키를 입력 받아야 합니다.)
		
		
		int height;
		Scanner sc = new Scaaner(System.in);
		height = sc.nextint();
		System.out.println("Your height is " + height+"cm");
		
```



```
int main(){

 double num,num1;

 char a;

 scanf("%lf %lf %c",&num,&num1,&a);

 printf("%.2lf\n%.2lf\n%c",num,num1,a);

}



float num1,num2;

double num3;

scanf("%f %f %lf",&num1,&num2,&num3);

printf("%.3f\n%.3f\n%.3lf",num1,num2,num3);

}


//형성평가 5 정올 110


 double yd;
  Scanner sc = new Scanner(System.in);
  System.out.printf("yard? ");
  yd = sc.nextDouble();
  System.out.printf("%.1fyard = %.1fcm", yd, yd * 91.44f);
  
  
```



