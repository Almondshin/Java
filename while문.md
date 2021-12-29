# while문

### while문이란? (반복문)
* 반복문은 어떠한 것을 반복적으로 사용하고 싶을 때 사용 한다
* 반복문의 종류는 while문, do-while문, for문 이 있다
* 조건문의 실행 결과가 true일 동안만 반복해서 실행한다. 
```
   while(조건문)
   {
     실행문;
   }
```
---
  - 10번 반복하면서 0부터 9까지 출력
```Java
public class Java
{
  public static void main(String[] args)
  {
    int i = 0; // 변수 선언
    
    while (i<10) // i가 10보다 작을 때 까지 반복해서 실행한다
    {
      System.out.println(1);
      i++; //조건문을 원하는 만큼만 반복하고 빠져나가기 위한 부분 
    }
  }
}

```
  - 1부터 100까지의 합

```Java
public class Java
{
  public static void main(String[] args)
  {
    int total = 100;
    int i = 1;
    
    while (i <= 100)
    {
      total = total + i;
      i++; //i를 하나씩 증가 시킬 값
    }
    
    System.out.println(total);
  }
}

```

### do while문이란?
* do while문의 경우는 무조건 한번은 실행되는 반복문이다
* Scanner는 java.util 패키지에 있는 클래스로써 키보드로 부터 값을 입력받는다던지 할 때 유용하게 사용할 수 있는 클래스입니다.

```Java
import java.util.Scanner

public class Java
{
  public static void main(String[] args)
  {
   int value = 0;
   Scanner scan = new Scanner(System.in); // 키보드로 부터 값을 입력받는 클래스 (Scanner)
   do
   {
      value = scan.nextInt(); // 정수값을 입력받아서 value에 넣어줌
      System.out.println("입력받은 값 : "+ value);
      //반복될 문장들
   }
      while(value != 10); // value가 10이 아니라면 계속 실행하고 싶어요
      
      System.out.println("반복문 종료!");
  }
}

```

