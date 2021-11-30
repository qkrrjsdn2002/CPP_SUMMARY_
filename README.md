클래스 상속의 매개변수 전달 방식

생성자는 지정된 기본 클래스 순서대로 실행되며 소멸자는 역순으로 실행된다.


가상 함수

상속 받은 클래스의 함수 중 하나를 수정하여 부모의 함수가아닌 자신의 함수를 실행하는 것

클래스의 멤버함수 앞에 virtual 이라는 키워드를 사용

ex) class DOG{ 
virtural char hi(char a){}
:
};


가상 함수 구현

클래스 멤버함수와 동일한 함수를 파생 클래에서 재정의 하여 사용하며 함수의 리턴값, 매개변수의 개수, 자료형이 모두 일치하여야한다.

또한, 이러한 가상함의 구현을 중복이라고 한다.


바인딩

변수와 함수의 메모리할당이나 함수 호출을 처리하는 명령어들이 결정되는 시점


정적바인딩

컴파일시 명령이 결정되는 경우


동적 바인딩

실행할 때 결정되는 경우
