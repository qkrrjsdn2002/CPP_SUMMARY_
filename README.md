객체의 멤버 호출
######
class Cat{

private:// 접근 속성

int Weight;// 멤버 변수

public:

int getWeight();// 멤버 함수

}; 

Cat Marry, *pNavi;// 객체

Marry.getWeight();// 일반객체가 멤버변수나 함수에 점근하기 위해 [클래스.멤버함수] 와 같은 형태를 취함

pNavi->getWeight();//포인터 객체가 멤버변수나 함수에 점근하기 위해 [클래스->멤버함수] 와 같은 형태를 취함

######
배열
######
연속적인 항목들이 동일한 크기의 순서를 갖고 나열되는 데이터의 집합

######
일차원배열
######

int 변수[배열의 개수] ex) int num[4]

num 배열은 정수형 자료 4개(0 ~ 배열의 개수-1 의 범위)를 저장 할 수 있는 공간을 가지게된다.


######
일차원 배열의 초기화
######

int num[4] = {10,20,30,40};// 하나의 변수와는 달리 여러 원소를 가지고 있기떄문에 중괄호로 묶음

######
문자형 배열의 초기화
######

char name[] = {'h','i','\0'}


배열의 선언과 초기화를 동시에 할시 원소의 개수 3은 생략 가능

배열의 마지막 원소는 항상 널문자인 '\0' 을 사용

아래와 같이 문자열 형태로도 초기화 가능

char name[] = "hi";

마지막 문자는 널 문자가 자동으로 할당되므로 원소의 개수는 3개

int num[100] = {1,2) 와 같은 배열을 작성시 num0, num1 은 작성된 값을 가지지만 나머지 원소들은 모두 0으로 자동 초기화


######
다차원 배열
######

int num [3][4] 인 배열의 크기는 3x4인 12의 크기를 가지고 마지막 원소는 num[2][3] 이다.

######
문자열 관련 함수
######

strcpy(abc,cba);// 문자열 cba를 abc로 접속

strcat(abc,cba);// 문자열 cba, abc를 연결

strcmp(abc,cba);// 문자열 abc, cba를 비교

strlen(abc);// abc의 길이

######
생성자와 소멸자
######

사용자가 정의하지 않아도 되는 멤버 함수

생성자는 주로 멤버 변수의 초기화를 한며 객체가 생성될때마다 자동으로 호출된다.

소멸자는 객체가 소멸될 때 자동으로 호출된다.

######
this 포인터
######

자동적으로 시스템이 만들어 주는포인터로 멤버가 호출될 때 해당 멤버가 속한 객체를 가르킨다.

클래스의 멤버함수 내에서 다른 클래스에 자기 자신을 매개변수로 넘길 때 주로 

Dog::~Dog()

{
cout<<"소멸";
}

int Dog::getAge()

{ 
return age; 
}

void Dog::setAge(int a)

{
age=a; 
}




