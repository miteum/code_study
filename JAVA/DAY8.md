# DAY8 #



순서도! 



---





## 객체 ##

> 객체란 



### 클래스 ###

> 객체의 생성의 가장 첫 번째 단계는 클래스 생성 
>
> 





## 자판기 만들기 ## 



```
public static void main(String[] args) {
		
		//변수 선언 및 초기화 (변수에 저장된 값) 
		final String[] beverageNames= {"콜라","갈아만든배","포카리"};
		final int[] beverageCost= {1100,1200,1400};
		final int[] beverageStock = {5,6,2};
		
		int money = 0;
		int selectedBeverage = -1;
		int isExit = 0;
		
		
		do {
			//반복횟수 명확 for문 사용
			for(int index=0; index <3; index++) {
                System.out.printf("%d.%s (%s원)\n",
                        index, beverageNames[index], beverageCost[index]);
            }
			
		do {
			//투입금액 입력 받기 위해 
			Scanner scanner = new Scanner(System.in);
			System.out.println("돈을 투입해 주세요");
			money = money+ scanner.nextInt();
		
			
			do {
				System.out.println("음료를 선택해주세요");
				selectedBeverage = scanner.nextInt();
				if(beverageStock[selectedBeverage] <= 0) {
					System.out.printf("%s 음료가 존재하지 않습니다. 다른 음료를 선택하세요.\n",
							beverageNames[selectedBeverage]);
						
				}
				
			}while(beverageStock[selectedBeverage] <=0);
			
			//음료가 존재하지 않는 경우 (조건문) 
			if(beverageCost[selectedBeverage]> money) {
				System.out.println("금액이 부족합니다.");
			}
			
		}while (beverageCost[selectedBeverage] > money);
		
		//잔고차감 및 재고차감 
		money = money - beverageCost[selectedBeverage];
		beverageStock[selectedBeverage] = beverageStock[selectedBeverage]-1;
		
		//음료구매 후 잔액 출력 
	    System.out.printf("%s 음료를 구매했습니다.\n", beverageNames[selectedBeverage]);

        System.out.printf("남은 금액은 %d원 입니다.\n", money);

        System.out.println("거스름 돈을 반환 받으시겠습니까?(yes는 1/ no는 0)");
        Scanner scanner = new Scanner(System.in);
        isExit = scanner.nextInt();
		}while (isExit == 0); 
	

	

```





```

public class Ex01 {
	
	//멤버변수 = 클래스내에 선언된 변수 ( 인스턴스변수와 정적변수) 
	String name;   //인스턴스 변수 
	int age;	//인스턴스 변수
	String id;  //인스턴스 변수
	static String nationality = "korea"; // 정적변수 
	
	
	public static void main(String[] args) {
		
		
	// 인스턴스를 생성 후에 접근 가능한 변수 = 인스턴스 변수 
		
		Ex01 per = new Ex01();
		
		per.name="김연경";
		per.age=34;
		
		System.out.println(per.name);
		
	}

}
```

