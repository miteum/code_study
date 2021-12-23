# DAY6

>
>
>프로그래밍을 잘 하는 방법



해답을 찾는게 아니라, 푸는 과정을 생각해보자

> 
>
> 1~10까지, 짝수를 구하라

```
    int number = 1;
        do {
            if (0 == number % 2) {
                System.out.println(number);
            }
            number = number + 1;
        } while (number <= 10);
    }

```





내가 생각한 코드 

```

for(int i = 1; i<=10; i++){
	if( i % 2 ==0 ){
     }else{
          i++;
          System.out.println("sum : "+ i);
   }         
 }
```

