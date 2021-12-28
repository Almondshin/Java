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
      i++; // i = i + 1;
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
