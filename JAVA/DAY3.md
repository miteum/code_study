# DAY3 #

*배열*

> 순서대로, 특정상자에 접근하기 위해



{0, 1, 2, 3, 4} > 0부터 시작하며, Index 라고함 



* 공간을 저장하는 방법 3가지 

```
int [] box = {10,20};
int [] box = new int[] {10,20};
int [] box = new int[2];
box[0] = 10;
box[1] = 20
```





* 읽는 법 

```
int [] box = new int [3];

box[0] = 10;
box[1] = 20,
box[2] = 30; 
```





# 다차원 배열 

> 2차원 배열, 3차원 배열 등 똑같은 개념이라고 보면 된다. 



* 2차원 배열 : 1차원 배열이 여러개라고 생각하자.

  ``` 
  char [][] page = new char[상위][하위]
  
  
  char[][] box = {
   {'1','p','a','g','e'};
  }
  
  page[0][0] ='1',
  page[0][1] ='p',
  page[0][2] ='a',
  page[0][3] ='g',
  page[0][4] ='e',
  
  ```

* 3차원 배열 

  ```
  char [][][] page = new char [최상위][상위][하위]
  ```

* 공간만 할당 후 값을 넣는 방법

``` 
char[][] page = new char[3][5]; 

page[0][0] = '1'; 
page[0][1] = 'p';
page[0][2] = 'a';
page[0][3] = 'g';
page[0][4] = 'e';

page[1][0] = '오';
page[1][1] = '늘';
page[1][2] = '공';
page[1][3] = '부';
page[1][4] = '는';


page[2][0] = '어';
page[2][1] = '떤';
page[2][2] = '걸';
page[2][3] = '할';
page[2][4] = '까';
```





# 배열과 메모리

* 배열변수 :  배열공간에 접근 할수 있도록 
* 배열 공간 :  데이터를 저장하는 공간 



``` 
첫 번째 주소 + ( 인덱스 * 자료형의 크기 ) => 접근할 주소 
```

배열공간의 첫번째 주소를 알고 있고, 배열에 저장되는 자료형을 알고 있다면 인덱스를 이용하여 특정 공간에 접근 할수 있음 



