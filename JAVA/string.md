



## 문자열 생성

```java
// 문자열 상수
String name = "포도";

// String 객체를 이용하여 생성
String name = new String ("포도");

// String 객체를 이용하여 생성
String name = String.format("%s도", "포");

// String 객체를 이용하여 생성
String name = String.join("%s%s", new String[] {"포", "도"});

// StringBuilder 객체를 이용하여 생성
String name = new StringBuilder().append("포").append("도").toString();

// StringBuffer 객체를 이용하여 생성
String name = new StringBuffer().append("포").append("도").toString();

// 문자열 상수를 더하여 생성
String name = "포"+"도";

// 변수에 저장된 문자열 상수와 문자열 상수를 더하여 생성
String text = "포";
String name =  text+"도";
```

출처: 코드라떼 

