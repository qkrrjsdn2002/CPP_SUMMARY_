입출력 객체

C++에서도 C에서 사용했던 stdio.h 파일의 입출력 함수를 이용할 순 있지만

C++에선 객체지향 중심의 입출력 스트링 함수가 있다.

스트림 함수는 사용자가 %s,%d 와 같은 형을 지정할 필요없이 자동 변환된다는 장점이 있다.

ex) cout << 변수 ; // 출력 함수
    
    cin >> 변수명 ; // 입력 함수
    

ios 클래스

istream 클래스는 입력 기능이 정의된 클래스

ostream 클래스는 출력 기능이 정의된 클래스

iostream 클래스는 istream 과 ostream 으로부터 다중 상속된 파생 클래스

ifsteram, ofstream, fstream 은 전체적인 기능인 위의 클래스들과 유사하지만 파일 입출력을 다룬다.


<< 연산자 중첩

cout을 쓰기 위해 사용한 << 연산자는 아래와 같은 형태의 여러개의 자료형으로 중첩 정의되어있다.

ex) basic_ostream& operator<<(자료형);


형식 입출력

c++의 입출력 형식을 지정하는 형식상태는 형식 플래그의 값에 의해 의미가 지정된다.

ex)

long setf(long f); // 플래그 세트 함수

long unsetf(f); // 플래그 클리어 함수

long flags(); // 플래그 참조 함수

long flags(long f); // 플래그 참조 함수

long setf(f1, f2); // 플래그 세트 함수


setiosflags() / resetiosflags()

특정한 형식 플래그를 설정하고 싶을 때 setiosflags() 함수를 사용

플래그를 사용하지 않으기 위해서는 resetios flags 함수를 사용하며 unsetf 함수와 동일한 기능을 가진다.








