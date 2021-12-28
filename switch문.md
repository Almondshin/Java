# switch문

### switch문이란?
* 어떤 변수의 값에 따라서 문장을 실행할 수 있도록 하는 제어문이다.
  - switch문에서 사용하는 키워드는 switch, case, default, break 이다.
  - case의 성질은 만난 케이스부터 나머지를 모두 실행한다.
  - if else처럼 사용하고 싶으면 break를 써야 한다.
  
  ```java
  public class Java
  {
    public static void main(String[] args)
    {
    // switch, case, default, break
    
    int value = 1;
    int test = 10;
    
    switch(value)
   {
      case 1:
        System.out.println("1");
      case 2:  // value가 2라면 만난 케이스부터 나머지를 모두 실행한다.
        System.out.println("2");
      case 3:
        System.out.println("3");
      default :
        System.out.println("그 외 다른 숫자");
    }
    
   switch(test)
   {
      case 10:
        System.out.println("10");
        break;
      case 20:  
        System.out.println("20");
        break;
      case 30:
        System.out.println("30");
        break;
      default :
        System.out.println("그 외 다른 숫자");
    }
    }
  }
  ```
