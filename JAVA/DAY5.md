# DAY5

>
>
>조건문 if, swich문에 대해서 

# 조건문 #

* if : 순차적으로 확인하여 '참'인 조건식을 만나면 조건문 내부에 있는 코드를 실행 후, 조건문을 탈출

``` 
if(조건식1) {
내용 A 
}else if(조건식2) {
내용 B
}else{
내용 
}

```



* switch 문 : 조건값에 따라 특정 case 부터 실행 할수 있도록 하는 구문 

```
switch (조건값) {
    case 값1 :
        // 조건값이 '값1'이면 해당 위치 부터 실행 후 아래의 case로 진행
    case 값2 :
        // 조건값이 '값2'이면 해당 위치 부터 실행 후 아래의 case로 진행
    case 값3 :
        // 조건값이 '값3'이면 해당 위치 부터 실행 후 아래의 case로 진행
    default:

}
```



[실습하기]

``` 
int num = 65;
char alphabet;

if (65 == num) {
    alphabet = 'A';
} else if (66 == num) {
    alphabet = 'B';
} else if (67 == num) {
    alphabet = 'C';
} else {
    alphabet = '0';
}

System.out.println(alphabet);
```



```
char locationPrefix = 's';

String location = "어딘지모름";

if ('k' == locationPrefix) {
    location = "강남";
} else if ('s' == locationPrefix) {
    location = "수원";
} 

System.out.println(location);
```





---

- **switch문**

조건값에 따라 특징 csse부터 실행 할 수 있도록 하는 구문, 특정 case부터 아래로 내려가며 코드를 실행 하되, break 키워드를 만나면 swich문을 탈출

 

 

 

-break 키워드 없는 switch 구문

 

 

```
switch (조건값) {
    case 값1 :
        // 조건값이 '값1'이면 해당 위치 부터 실행 후 아래의 case로 진행
    case 값2 :
        // 조건값이 '값2'이면 해당 위치 부터 실행 후 아래의 case로 진행
    case 값3 :
        // 조건값이 '값3'이면 해당 위치 부터 실행 후 아래의 case로 진행
    default:
 
}
```

 

-조건값이 '값1' 이면 case 값1 > case 값2 > case 값3 > defalult 순으로 실행

-똑같이 실행 후 switch 문을 탈출 하지 않는 이상 default는 맨 마지막에 실행 

 

 

------

 

-break 키워드 있는 switch 구문

 

```
switch (조건값) {
    case 값1 :
        // 조건값이 '값1'이면 해당 위치 부터 실행 후 탈출
        break;
    case 값2 :
        // 조건값이 '값2'이면 해당 위치 부터 실행 후 아래의 case로 진행
    case 값3 :
        // 조건값이 '값3'이면 해당 위치 부터 실행 후 아래의 case로 진행
    default:
 
}
```

 

 

-break 키워드 있는 switch 구문1

```
switch (조건값) {
    case 값1 :
        // 조건값이 '값1'이면 해당 위치 부터 실행 후 탈출
        break;
    case 값2 :
        // 조건값이 '값2'이면 해당 위치 부터 실행 후 아래의 case로 진행
    case 값3 :
        // 조건값이 '값3'이면 해당 위치 부터 실행 후 아래의 case로 진행
    default:
 
}
```

 

 

-break 키워드 있는 switch 구문2

```
switch (조건값) {
    case 값1 :
        // 조건값이 '값1'이면 해당 위치 부터 실행 후 탈출
        break;
    case 값2 :
        // 조건값이 '값2'이면 해당 위치 부터 실행 후 아래의 case로 진행
    case 값3 :
        // 조건값이 '값3'이면 해당 위치 부터 실행 후 탈출
        break;
    default:
 
}
```

 

 

 

-break 키워드 있는 switch 구문3

```
switch (조건값) {
    case 값1 :
        // 조건값이 '값1'이면 해당 위치 부터 실행 후 탈출
        break;
    case 값2 :
        // 조건값이 '값2'이면 해당 위치 부터 실행 후 탈출
        break;
    case 값3 :
        // 조건값이 '값3'이면 해당 위치 부터 실행 후 탈출
        break;
    default:
 
}
```

 

 

-default 키워드 없는 switch 구문

```
switch (조건값) {
    case 값1 :
        // 조건값이 '값1'이면 해당 위치 부터 실행 후 탈출
        break;
    case 값2 :
        // 조건값이 '값2'이면 해당 위치 부터 실행 후 탈출
        break;
    case 값3 :
        // 조건값이 '값3'이면 해당 위치 부터 실행 후 탈출
        break;
}
```

---



# 반복문



for :  대체로 반복할 횟수가 정해져 있을 때 사용

``` 
for( 초기화; 조건식; 반복 후 실행될 명령어) {
//반복 시킬 내용
}
```



```
* for문을 이용해 3의 배수의 총합을 구하라 
 
public static void main(String[] args) {
int num = 0;
		
		
		for(int z = 1; z<= 100; z++ ){
			if(z% 3 ==0 ) {
				num += z;
			
			}
		}
	
		System.out.println("3의 배수  " +  num);
	}
	}

```







```
for(int num = 0; num <4; num++) {
System.out.println(num);
}

결과 : 
0
1
2
3
```





while : 대부분 반복할 횟수가 정해져 있지 않을 때 사용

``` 
while (조건식) {
//반복 시킬 내용
}
```





do ~ while : 반복할 횟수가 정해져 있지 않고, 조건 여부 상관없이 먼저 코드 실행 후 반복할 때 사용 

```
do {
//반복 시킬 내용
}while(조건식);
```





