# for문

### for문이란?
* for 반복문은 변수초기화, 조건식, 증감식으로 구성 되어있다.
  - 1. 초기화식은 최초 한 번만 수행합니다.
  - 2. 조건식이 true라면 실행문을 수행한다
  - 3. 증감식을 수행한다
  ```
  for(변수 선언 초기화 (초기화식); 반복여부를 결정하는 판단문 (조건식); 반복상태 정보갱신 (증감식))
  {
    실행문;
  }
  ```

  ```Java
  public class Java
  {
    public static void main(String[] args)
    {
      int total = 0;
      
      for(int i = 1; i <= 100; i++)
      {
        if(i % 2 != 0)  // 2로 나눈 나머지가 0이 아니라는것은 홀수를 의미한다. 
        {
          continue; // continue를 만나면 그 아래쪽에 반복문에 해당하는 부분을 실행시키지 않고 증감식으로 올라간다.
        }
        total++;
      }
      System.out.println(total);
    }
  }
  ```

  ```Java
  public class Java
  {
    public static void main(String[] args)
    {
      int total = 0;
      
      for(int i = 1; i <= 100; i++)
      {
        if(i % 2 != 0)  // 2로 나눈 나머지가 0이 아니라는것은 홀수를 의미한다. 
        {
          break; // break를 만나게되면 반복문을 빠져나온다.
        }
        total++;
      }
      System.out.println(total);
    }
  }
  ```
