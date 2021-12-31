package mc.ys.lesson2;

import java.util.Scanner; // Scanner 클래스를 사용하기 위해 추가

public class CalendarGY 
{

	public static void main(String[] args)  // 실행 메소드
	{
		//실행메소드(main메소드) 외부에서의 호출할 때에는 인스턴스화 시켜야 한다.
		CalendarGY cm = new CalendarGY(); //< 클래스명 참조변수(변수명) = new 클래스명(매개변수); >
		cm.start(); //< 참조변수(변수명).메소드(매개변수) > cm이 가지고있는 start를 실행시킨다
	}
	
	// static이 없으면 instance에서만 호출 할 수 있다
	// 매개변수가 없는 생성자는 컴파일러가 자동으로 기본생성자를 추가해준다.
	// 메소드 이름의 첫번째 글자는 소문자로 적는다. 이어지는 문자의 경우 뒤의 문자의 첫번째 글자를 대문자로 써준다. 언더바 사용하지 않는다.
	
	// 이름은 start인 리턴을 하지않고 공개되어있는 메소드입니다.
	public void start() // 메소드 start가 매개변수가 없는 생성자기 때문에 소괄호를 비워둔다
	{
		Scanner scan = new Scanner(System.in); // Scanner 클래스 객체 생성
		boolean flag = false; // 하드코딩 되어있던 while문에 들어가는 변수
		while(!flag) 
		{
			System.out.print("input month please >>> ");
			int cmd = scan.nextInt(); // 정수를 입력받아 변수 cmd에 저장
			
			//메소드가 리턴값이 없는경우 < 메소드(매개변수); >으로 호출 가능하다
			makeCalendar(cmd); //클래스 내부에서의 다른 메소드를 호출 
			
			System.out.print("be continue? [Yes:1, No:0] >>> ");
			cmd = scan.nextInt();
			if(cmd==0)
			{
				System.out.println("Calendar Service is Stop!!");
				flag = true;
			}
		}
		scan.close(); //오픈할때마다 닫는것?
	}
	
	// 이름은 makeCalendar입니다 int형의 변수를 선언했고 리턴을 하지않고 공개되지 않은 메소드입니다 
	//(공개되어있지 않은 메소드는 같은 클래스에서만 사용 가능하다)
	void makeCalendar(int mon)  //retrun값이 없다. = 기능을 꺼내와서 사용하지 않고 이 메소드 안에서 끝낸다.
	{
		int year = 2021;
		int month = mon;
		int[] spaces = new int[12];
		int[] lastDays = {31,28,31,30,31,30,31,31,30,31,30,31};
		spaces[0] = (2+31)%7;
		for(int i=1;i<12;i++)
		{
			spaces[i] = (spaces[i-1]+lastDays[i-1])%7;
		}
		
		int space = spaces[month-1];
		//윤년판단 로직
		int lastDay = lastDays[month-1];
		if(year%400==0 || (year%4==0&&year%100!=0)) 
		{
			lastDay = 29;
		} 
		
		System.out.printf("%d년 %d월 %n",year,month);
		System.out.println("일\t월\t화\t수\t목\t금\t토");
		for(int i=0;i<space;i++)
		{
			System.out.print("\t");
		}
		int day = 1;
		//    
		for(int i=0;i<lastDay;i++) 
		{ 
			System.out.print(day+"\t");
			if((space+day)%7==0) 
			{
				System.out.println();
			}
			day = day + 1;
		}
		
		System.out.println("\n");
	}
	
	

}
