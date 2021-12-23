# DAY7 #

> 문자열을 만들고 문자열을 출력하는 다양한 방식에 대해서 



원하는 문자를 출력하기 위해서 문자열을 반환하는 메서드

String.format 

```
String name = "랄라"

String output = String.fotmat("내 이름은 %s 이다", name);
System.out.println(output);


출력
내 이름은 랄라 이다
```

* %s는 일반적으로 문자열을 대입해주는 지정자





format 지시어 

* %a  > 부동소수점 타입  > 16진법 문자열
* %b > 모든 타입 >  boolean 값은 true, false , 참조 자료형인 경우 null이면 false, not null이면 true
* %c > 문자 타입 >  유니코드 문자
* %d > 정수 타입 > 10 진법 문자열
* %e > 부동 소수점 타입 > 과학적 표기업(e)를 이용한 10진법 문자열
* %f > 부동 소주점 타입 > 10진법 문자열
* %g > 부동 소수점 타입 > 수의 표현 범위가 넓어지면 과학적 표기법(e)를 이용한 10진법 문자열
* %h > 모든 타입 > hashCode 값으로부터 16진법 문자열
* %o > 정수 타입 > 8진법 문자열
* %s > 모든 타입 > 문자열 값
* %t > Date / Time
* %x > 정수 타입 > 16진법 문자열





​																																																						