# if문

### if 조건문
* 조건식의 연산 결과에 따라 블록 내부 문장의 실행 여부를 결정 할 수 있다.
  - if문
    - 조건식이 true 일 경우에만 실행문이 실행된다
    ```Java
    public class Java
    {
      public static void main(String[] args)
      {
        int x = 50;
        int y = 60;
        
        if (x < y)
          {
            System.out.println("x는 y보다 작습니다");
            System.out.println("Test");
          }
        
      }
    }
    ```
  - if - else
    ```Java
    public class Java
    {
      public static void main(String[] args)
      {
        int x = 50;
        int y = 60;
        
        if (x == y)
          {
            System.out.println("x는 y와 같습니다"); // 위 조건에 만족했다면 실행된다
          }
          else
          {
            System.out.println("x와 y는 다릅니다"); // 그러지 않았다면 else블럭 안에 있는 부분이 실행된다
          }
      }
    }
    ```
   - if - else if - else문
    ```Java
    public class Java
    {
      public static void main(String[] args)
      {
        int x = 50;
        int y = 40;
        
        if (x == y)
          {
            System.out.println("x는 y와 같습니다"); // 위 조건에 만족했다면 실행된다
          }
          else if (x < y)
           {
             System.out.println("x는 y보다 작습니다"); // 그러지 않았다면 else if블럭 안에 있는 부분이 실행된다
           }
           else
           {
            System.out.println("x는 y와 다릅니다"); // 그러지 않았다면 else블럭 안에 있는 부분이 실행된다
           }
      }
    }
    ```
