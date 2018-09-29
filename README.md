# interviewpc


- 아이폰 개발 시작동기와 학습 방법
프로그래밍을 해보자고 생각했을때 하드웨어가 완성되어 있는 상태면 좋겠다는 생각을 했었습니다.  그걸 사용해서 하드웨어의 특징을 살려서 좋은 기능을 구현해 볼수도 있을것 같았고 지금 만들어져있는 어플들을 많이 사용하고 있는데  이 경험을 살려 더 좋은 서비스를 만들어 낼수 있을것 같다는 생각이 들어서 아이폰 개발을 시작하게 되었습니다.


- 주로 사용하는 패턴이나 좋아하는 개발 방법론과  그 이유
지금은 MVC 패턴을 사용하려고 노력하고 있습니다. 이유는 Swift에서 기본적으로 알아야 되는 패턴이라고 생각이 들어서입니다. 지금 관심이 있는 패턴은 MVVM인데 공부를 제대로 해서 실제로 사용을 해보고 싶습니다. 개발 방법론은 개인적으로는 페어프로그래밍에 대해서 관심이 좀 있습니다. 페어프로그래밍은 한 컴퓨터를 2명의 사용자가 사용하는 방식으로 알고 있는데 개발을 진행하면서 프로젝트를 하다보면 이게 최선인지 찝찝한 느낌 이 드는 부분들이 있을것 같은데 그때 바로바로 이야기 하면서 해결을 빨리 할수 있을것 같고 개인적으로 가지고 있을수도 있는 나쁜 습관들을 고칠수 있을수도 있다고 생각하기 때문입니다.

- Hybrid 앱 개발 경험이 있는가 ?

없습니다.

- OpenURLScheme을 사용해 보았는가?
오픈 URL을 사용해서 셋팅화면이나 메일을 사용하는 예제를 만들어 본적이 있으며, 페이스북도 화이스리스트를 등록해서 사용해봤습니다.

- 앱스토어 배포 경험이 있는지?
없습니다. 

- 블록, 넌블럭, 동기, 비동기의 차이는?
블럭 - A라는 함수를 호출 했을때 행위를 모두 끝마칠때까지 기다리는걸 말합니다.
논블럭 - 함수를 호출 했을때 기대하는 어떤 행위를 요청하고 바로 리턴되면 논블럭킹되었다고 합니다.
동기 비동기는 A와 B라는 함수가 있을때 A가 실행되고 B가 실행되면 동기, A와 B가 동시에 실행되면 비동기라고 볼수 있을것 같다

- GCD가 무엇인지?
GCD는 애플에서 만든 스레드 관리와 실행에 대한 책임을 운영체제 레벨에서 관리하도록 한 기술입니다. 작업의 단위를 블럭으로 나누며 DispatchQueue가 블럭을 관리하는걸로 알고 있습니다.
sync 동기, async 비동기
sync 동기, async 비동기
DispatchQueue.main.async { }
DispatchQueue.global().async { }
DispatchQueue.global().sync { }


- 샌드박스란 무엇이고 왜 샌드박스를 사용하는지?
한정적인 공간안에서 놀수 있게 하는 대신 외부에서는 하지 못하도록 틀을 만들어 가지고 있는걸 샌드박스 라고 하는것 같습니다. 샌드박스는 앱에 허용된 자원만 접근이 가능하게 의도적으로 막아 공격을 어렵게 하기 위한 시스템이기 때문에 보안면에서 좋은것 같습니다.

- 당신의 꿈은 무엇인가요? 정말 솔직한 자신의 꿈을 말해주세요.
저의 꿈은 60살이 넘어서까지 코딩을 하는 사람이되는 것입니다. 

- 최근 동향이나 소식은 어디를 통해 접하는지?
구글 얼럿을 사용하거나, 스위프트 관련 이슈를 매주 보내주는 사이트에서 메일을 받아봅니다.

- iPhone5/5s, iPhone6, iPhone6+ 스크린 단편화에 대한 대응은 어떻게 할 것인지?
오토레이아웃을 더 적극적으로 활용해서 반응형으로 만드는게 좋다고 생각합니다.

- 개발을 하다가 막히는 부분은 어떻게 해결하는지?
애플 개발자 문서를 읽어보고 해결이 안되면 가지고 있는 책을 참고하거나 스텍오버플로우에 검색을 합니다.

- 좋은 회사란? 어떤 회사라고 생각하는지?
회사에 가는 시간이 즐거워진다면 좋은 회사라고 생각합니다.

- ARC가 무엇이며 동작 원리는?
ARC는 Reference count를 자동으로 관리해주는 방식으로 컴파일러가 개발자를 대신해서 메모리 관리 코드를 적절한 위치에 삽입합니다.
ARC는 Reference 할때만 RC 카운터가 올라가기 때문에 레퍼런스 타입인 class의 인스턴스에만 적용된다고 봐도 됩니다.
Struct나 Enum과 같은 Value타입은 적용되지 않습니다.

- 스레드와 프로세스의 차이점
프로세스는 운영체제에서 실행중인 하나의 프로그램을 말하고 스레드는 프로세스에서 실행되는 각각의 일을 말합니다.
기본적으로 프로세서는 하나의 스레드를 가지고 있는데 그 스레드를 메인 스레드라고 합니다. 1개 이상의 스레드가 있을때는 멀티스레드 라고 합니다.
프로세스는 Code, Data, Heap, Stack을 가지고 있으며, 각각의 메모리 공간을 차지하고 있습니다.
스레드는 프로레스의 안에서 동작하고  Code, Data, Heap는 공유 Stack만 별도로 가지고 있습니다.
스레드는 메모리를 공유하기 때문에 독립적인 프로세스와 다르게 스레드간 데이터를 주고 받는게 간단하고, 시스템 자원 소모가 적습니다. 물론 응답시간도 단축이됩니다.

- OOP가 뭐고 특징이 뭐니?
Object-Oriented Programming
객체지향 프로그래밍은 추상화, 캡슐화, 상속성, 다형성을 이용하여 코드 재사용을 증가시키고, 유지보수를 감소시키는 장점을 얻기위해 객체들은 연결시켜 프로그래밍을 하는것을 말합니다.
추상화(Abstraction 업스트렉션) - 대상의 복잡성을 줄여서 목적에 집중할수 있도록 하는 단순화 작업
캡슐화(Encapsulation 인캡슐레이트) - 연관된 상태와 행동을 하나의 단위로 묶는 작업
데이터 캡슐화와 정보 은닉화가 있습니다.
은닉화(Information Hiding) - 외부에 필요한 것만 알리고 불필요 한거나 감줘야 하는 정보는 숨기는 작업
상속성(Inheritance 인히러텐스) - 부모의 클래스를 자식 클래스가 물려받아 부모 클래스의 기능을 동일하게 사용하는 것
Swift에서는 다중 상속을 비 허용


- OOP, POP 차이
Object-Oriented Programming, Protocol-Oriented Programming
OOP는 추상화, 캡슐화, 상속성, 다형성을 이용해서 상향식 접근법으로 프로그래밍을 하여, 코드 재사용을 증가 시키고 유지보수를 감소시킬려고 하는 프로그래밍 방법입니다.
POP는 하향식 접근법 따르며 Protocol과 extension을 통한 수평확장을 통해서 코드 재사용과 유지보수를 감소시킬려고 하는 프로그래밍 방법입니다.


-POP란 ? 
POP는 하향식 접근법 따르며 Protocol과 extension을 통한 수평확장을 통해서 코드 재사용과 유지보수를 감소시킬려고 하는 프로그래밍 방법입니다.


- Call by value(밸류 타입), Call by reference(참조 타입)
Call by value는 변수 할당시 Stack에 값 전체가 저장됩니다.
다른 변수에 할당될 때 전체 값이 복사되기 때문에 (Copy by value) 변수들이 분리되어 하나를 변경해도 다른 것에는 영향이 없습니다.
Heap을 사용하지 않기 때문에 RC는 필용벗지만 인자를 넘겨줄 때 마다 메모리 공간을 할당하기 때문에 메모리 공간을 좀 더 잡아먹게 됩니다. 대표적으로 struct가 있습니다.
Call by reference는 참조 할수 있는 메모리 주소를 사용해서 값에 접근합니다. 직접 접근하기 때문에 원본 데이터의 값을 변경할수 있습니다. 또 메모리 공간을 한번만 사용하기 때문에 메모리 할당 문제에서 벗어나게 됩니다. 대표적으로 class가 있습니다.

- 비동기식을 왜 썼니, 동기식이랑 무슨 차이니
동기식은 동시에 일어난다는 뜻으로 요청을 하면 시간이 얼마가 걸리든 요청한 자리에서 결과가 나와야 합니다.
비동기식은 동시에 일어나지 않는다는 뜻으로 요청을 하면 다른 스레드에 일을 시킨뒤 결과는 다음에 받고 다른 작업을 할수 있습니다.
데이터를 서버에서 받아오는 작업과 같이 종료되는데 시간이 걸리는 작업은 비동기식을 사용해 봤습니다.
  
- 배열과 ArrayList의 차이점
배열은 크기를 한번 정하면 크기를 변경할수 없습니다. 배열 초기화시에 메모리에 할당되어 있기 때문에 ArrayList보다 빠릅니다.
ArrayList는 크기가 가변적이고 데이터 추가 삭제가 가능합니다. 데이터를 추가하고 삭제하는 과정에서 메모리에 재 할당을 하기 때문에 속도가 배열보다 느립니다.

- JSON의 구조
객체를 중괄호({})로 표시하고 이름과 값의 쌍으로 만들수 있습니다. 배열은 대괄호([])를 사용해서 표현합니다.
(칠판이나 공책에 써주는게 좋을듯..)
{
   "name": "식빵",
   "family": "웰시코기",
   "age": 1,  
   "weight": 2.14
   "dog": [
     {"name": "식빵", "family": "웰시코기", "age": 1, "weight": 2.14},
     {"name": "콩콩", "family": "포메라니안", "age": 3, "weight": 2.5},
     {"name": "젤리", "family": "푸들", "age": 7, "weight": 3.1}
   ]
}


- XML,JSON의 차이점이 뭐니
XML은 작성이 편리하고 가독성이 좋으나 HTML과 같이 tag구조고 이루어져있기 때문에 문서의 양이 늘어 납니다.
JSON은 최소한의 정보를 담고 있어서 XML보다 가벼우나 함축적이기 때문에 가독성이 떨어질 수 있습니다.

- Static 키워드에 대해 설명하세요.
타입 프로퍼티 선언을 할때 사용하는 키워드입니다.
클래스, 구조체, 열거형에서 사용이 가능하며 클래스에서 사용할 경우 서브클래스에서 오버라이드를 할수 있습니다.

- 오버로딩과 오버라이딩 비교
오버라이딩을 재정의로 부모 클래스에 선언되어 있는 기능을 재정의 할때 사용합니다.
오버라이딩을 방지하려면 final 키워드를 사용합니다
오버로딩은 매개변수를 다르게 함으로써 메서드를 여러개 만드는것을 말합니다. 즉 같은 클래스내에서 같은 이름의 메서드를 사용할수 있습니다.

- OSI 7계층이 무엇인지 설명해 보세요.
컴퓨터 네트워크 프로토콜 디자인과 통신을 계층으로 나누어 설명한 것입니다.
물리계층
물리 계층(Physical layer)은 네트워크의 기본 네트워크 하드웨어 전송 기술을 이룬다.
데이터 링크 계층
네트워크 위의 개체들 간 데이터를 전달하고 물리 계층에서 발생할 수 있는 오류를 찾아내고 수정하는데 필요한 기능적 절차적 수단을 제공하는 계층으로 대표적으로 이더넷이 있습니다.
네트워크 계층
데이터를 연결하는 다른 네트워크를 통해 전달함으로써 인터넷이 가능하게 만드는 계층이다
전송 계층
전송 계층(Transport layer)은 양 끝단(End to end)의 사용자들이 신뢰성있는 데이터를 주고 받을 수 있도록 해 주어, 상위 계층들이 데이터 전달의 유효성이나 효율성을 생각하지 않도록 해준다.  대표적으로 TCP가 있습니다.
TCP는 IP가 처리할수 있도록 데이터를 여러개의 패킷으로 나누고 도착한 다음에는 완전한 데이터 패킷으로 조립합니다.
세션 계층
세션 계층(Session layer)은 양 끝단의 응용 프로세스가 통신을 관리하기 위한 방법을 제공한다
표현 계층
표현 계층(Presentation layer)은 코드 간의 번역을 담당하여 사용자 시스템에서 데이터의 형식상 차이를 다루는 부담을 응용 계층으로부터 덜어 준다
인코딩, 암호화 동작을 하는 계층입니다.
응용 계층
응용 계층(Application layer)은 응용 프로세스와 직접 관계하여 일반적인 응용 서비스를 수행합니다.

- 64비트와 32비트의 차이점은 무엇인가요?
비트는 CPU가 처리할수 있는 최소한의 데이터로 32비트는 2^32만큼 64비트는 2^64만큼 데이터를 처리 할수 있습니다.

- Mutable Immutable 객체에 대해서.
Mutable 객체는 객체내의 특정 요소를 변경 가능합니다.
Immutable 객체는 객체내의 요소를 변경할수 없습니다.

- weak / strong , assign/retain 의 설명과 차이점.
retain은 코드에서 메모리를 참조하려고 할때 레퍼런스 카운터가 증가하는걸 말합니다.
assign  객체의 retain count를 증가시키지 않는다. 외부에서 retain count를 감소시켜 객체를 소멸할수 있다.
strong - 객체에 접근 가능한 모든 연결을 끊었음에도 순환 참조로 인해 활성화된 카운터가 남아서 메모리 누수가 발생하는 현상
weak - 레퍼런스 카운터를 올리지 않고 참조를 해서 강한 순환 참조를 방지할수 있으머 메모리 해제시 nil을 반환합니다.

- Delegate 설명. 활용
자신이 할일을 다른 인스턴스에게 대신 처리하도록 하는 디자인 패턴입니다.
MVC 패턴에서는 View가 ViewController에게 말할때 사용하며, tableView, collectionView, textField의 상태에 따른 동작을 사용하고 싶을때도 사용할수 있습니다.

- Delegate / Notification 의 차이와 활용도
코드 길이의 차이
다수의 객체들에게 동시의 이벤트 발생을 알려 줄수 있냐 없냐
Notification은 Delegate에 비해 추적이 쉽지 않을 수 있음
Delegate는 커뮤니케이션 과정을 유지하고 모니터링 하는 NotificationCenter와 같은 제 3의 객체가 필요없습니다.

- 카테고리 확장과 / 서브 클래싱  이 둘에 차이와 각각의 활용도.
object-C 관련이라 구지 몰라도 괜찮을지도
카테고리 확장은 기존 정의된 클래스를 쉽게 확장할 수 있도록 합니다.
서브 클래싱은 기존 클래스에 새로운 속성을 부여하는 것으로 init()를 생각하면 됩니다.

- Swift 와 Objective - c 를 동일한 코드를 구현할때 서로간에 장점과 단점은?
코드를 더 간결하게 만들수 있다?
최신으로 추가되는 기능을 Swift에서 쉽게 사용할수 있다.

- ARC와 block, gcd와 연관해서 설명해보세요
ARC(오토메틱 레퍼런스 카운터), CGD(그랜드 센트럴 디스패치), block(GCD에서의 작업의 단위)
시불 관계가 있는건가 ㅡㅡ ;;

- NSArray, NSDictionary, NSSet의 쓰임
NSArray - 순서가 있고 0부터 시작 같은 값을 가질수 있습니다.
인덱스로 값을 찾아야 되는 상황일때 사용할 수 있습니다.
NSDictionary - 키와 값으로 이루어져 있고 순서가 있습니다.
유저 아이디나, 토큰값을 저장할때 사용할 수 있습니다.
NSSet - 순서가 없고 유니크한 값을 가집니다.
특정 개체가 있는지 확인 할때 사용할수 있습니다.

- delegate 프로퍼티를 assign속성을 주는 이유? ( Delegate 프로퍼티를 weak으로 하는 이유)
순환 참조를 막기 위해서 assign / weak을 사용합니다.
참조 카운터를 올리지 않았기 때문에 강한 순환 참조를 방지할수 있습니다.

- MVC패턴설명
Model, View, ViewController로 나누는 패턴으로 Model과 View는 대화를 할수 없고 View와 ViewController는 델리게이트, action을 통해서 대화하고, Model과 ViewController는 KVO, Notification으로 대화하는 걸 말합니다

- Auto release pool을 동작 설명
Autorelease는 실제 코딩시 생성한 객체들을 일일히 적절한 타이밍에 해제해 주는것이 어렵고 객체가 해제되는 시점을 사람이 정하는것도 쉽지 않아서 해제해야 할 객체들을 모아 놨다가 release를 하는걸 말합니다.
@autoreleasepool 키워드를 넣으면 실행 됩니다.

- 버전은 어디까지 커버가 가능한지
Swift4, iOS7

- alamofier없으면 뭐쓸건지
AFNetworking을 사용하거나 URLSession을 사용해서 구현하겠습니다.

- 오브젝티브c볼줄아냐 (버전관리때문에 )
능숙하진 않지만 수업때 예제들을 간간히 배웠고 읽을 수는 있습니다. 그리고 Swiftify같은 프로그래을 활용 할 수 있다.

- Codable 이전에는 어떻게 파싱했을까
Swift3에서는 SwiftyJSON을 사용할것 같습니다. 

- app life cycle
Not running -> Inactive -> Active -> background -> Suspended -> 제거
Not running -> Inactive -> Active -> background -> Inactive
Inactive + Active를 Foreground 라고 함
ㅡ.ㅡ 이거는 음 어디서 무슨메서드가실행되나 그런게아니라 포어그라운드 뭐그라운드해서 기본베이스지식이필요 

- NSString *b = @"test";
NSString *a = [b copy]; 
에서 a와 b는 같은가? (주소값 포함)


- WWDC 세션중 관심있게 보는 세션은 어떤것이 있는가? 신기술 습득은 어떤 식으로 하는가
midium과같은 기술블로그나, 매주마다 ㅇㅇ위클리ㄹ를 통해서 최신정보를 습득한다.

- push 서비스 등록시 절차과정
APP ID에 푸쉬서비스 등록, 푸쉬 인증서 발급, 앱에 알림권한 획득을 위한 코드추가, Provider서버 구축 등등.



- 스택과 링크드리스트와 리스트의 차이점을 설명해 보세요.


- 팀프로젝트를 하면서 너는 어느부분을 맡았니, 어려움은 없었니
배민찬을했는데 상세페이지부터 - 


- SVC이나 git써봤니
git과 github를 사용해봤습니다.


- 다른 사람과 의견 충돌해본 경험, 그것을 어떻게 풀어갔나?


- 상단 상태바에 색깔을 변경하는 방법은?

- sdk란?

- restapi란?

- library란?

- rxswift란?

- mvvm, mvc, mvp패턴이란?








- Bubble Sort
var bubble = [5, 3, 7, 1, 6, 9, 2, 10, 13]
var count = 0

for count in 1...bubble.count {
    for idx in 0..<bubble.count - count {
        if bubble[idx] > bubble[idx + 1] {
            let value = bubble[idx]
            bubble[idx] = bubble[idx + 1]
            bubble[idx + 1] = value
        }
    }
}
print(bubble)

- selection Sort

var selection = [5, 2, 4, 6, 1, 3]

for number in 0..<selection.count {      // 0, 1, 2, 3, 4, 5
    print(number)
    for idx in 0...number {
        if  selection[idx] > selection[number] {
            let value = selection[number]
            selection[number] = selection[idx]
            selection[idx] = value
        }
        print(selection)
    }
}


- 2 이상의 정수를 입력받아, 소수인지 아닌지를 판별하는 함수

func primeNumber (num1: Int) -> String {
    guard num1 > 1 else { return "2이상의 정수를 입력하세요" }
    
    let number = [2, 3, 5, 7, 9] // 9이하의 약수
    
    for i in number {
        if num1 == 2 || num1 == 3 || num1 == 5 || num1 == 7 {
            return "\(num1)는 소수 입니다."
        } else if num1 % i == 0 {
            return "\(num1)은 소수가 아닙니다."
        }
    }
    return "\(num1)은 소수입니다."
}

for i in 0...100 {
    print(primeNumber(num1: i))
}



- 사용해본 iOS 개발 언어 ?	swift									
- Objective-C 프로젝트를 Swift로 이전한 경험이 있으신가요?	아니요									
- ARC와 non-ARC에 대한 개념을 이해하고 있다.  설명해보세요.	"종찬 : arc는 기존에 메모리 누수에 대해서 프로그래머가 따로 관리해줘야했던것과 달리  swift로 넘어오면서 자동적으로 컴파일러단에서 메모리 누스를 막아주는 걸로 알고있습니다.
이섭: - 네 . 기존 objective-C에서는 일일이 개발자가 변수생성할때나 초기화등 메모리 관리를 직접했었는데 , ARC 나오고 나면서 더이상 메모리 관리를 개발자가 할필요성이 없어졌어요.
뜽진 : iOS5 때부터 ARC라는 개념이 나옴. 그 전에는 객체에 대한 소유권을 가지고 있으므로 개발자가 스스로 메모리를 관리 해야했어야했는데 ARC가 도입되면서 더이상 retain / release / autorelease를 직접 삽입할 필요가 없어졌다. 컴파일러가 다 알아서 해준다."									
- Instruments를 활용하여 앱의 Memory 사용량을 확인하고 리팩토링해본 경험이 있다. 설명해보세요. 	뜽진 : 먼저 네비게이션의 디버그 부분에서 CPU와 Memory량을 확인 해본 후 메모리가 증가/감소 여부를 파악하며 문제가 있을시 Instruments를 이용해서 Memory Leak이 어느 부분에서 존재하는지 확인합니다.									
- Strong, Weak, Unowned의 개념을 이해하고, 사용하고 있다. 설명해보세요.	"뜽진 : Strong은 기본값이며 참조될 때마다 참조 카운트 1 증가하고,
약한 참조 (Weak), 미소유 참조 (Unowned) : 참조 카운트를 증가시키지 않습니다.
Weak와 Unowned의 차이점은 weak는 참조하던 객체가 해제될때는 nil로 바뀝니다. 
Unowned는 메모리 해제시에도 항상 메모리 주소 값을 가지고 있기 때문에 만약 참조중인 인스턴스가 해제된 unowned 참조 타입 프로퍼티에 접근하면 런타임 에러가 발생합니다.(요게 `댕글리포인터`라고 하는데 요거 찾아보세여 중요한 개념입니다.)
Unowned 참조는 댕글리포인터가 발생할 수 있기때문에 프로퍼티에 항상 인스턴스의 참조값이 있다고 보장될때만 사용해야합니다."									
- Restful API를 이용한 네트워크 연동 앱을 만들어 보았다. 설명해보세요.	"팀프로젝트로 카피앱을 진행 중에 네트워크 연동 앱을 진행했습니다. 백앤드팀에서 클래스 모델링과 restful api 명세서를 작성해주었고,
 ios 팀은 해당 url로 접속하여 파라미터나, 토큰등의 요구조건을 부합하면 데이터를 data타입으로 리스폰스 받는 방식으로 진행했습니다. 
받아온 데이터는 코더블또는 swiftjson, objectmapper등의 라이브러리를 이용하여 json형식으로 파싱하였습니다."									
- 네트워크 연동을 위해 Alamofire, AFNetworking등의 라이브러리를 사용해보았다. 각라이브러리는 왜사용했는지? 장단점?	"- 장희 : Alamofire : Swift, AFNetworking : Objecjt - C 둘다 HTTP로 하는 통신을 쉽게 해주는 라이브러리로 기능은 비슷한걸로 알고 있습니다. Swift로 동작하는 Alamofire만 사용해봄, 사용해 보진 않았지만 AFNetworking은 오래 되었기에 더 강력하 기능들이 많이 있다고 들음 하지만 알라모파이어는 최근에도 지속적인 업데이트를 하고 있고 신속하고 빠르게
동작하는걸 목표로 업데이트 되고 있는걸로 알고 있음"									
이미지를 Memory-Cache와 Disk-Cache를 이용해 캐쉬처리 해보았다. (오픈소스 사용 포함) 설명해보세요.	안해봤습니다.									
- GCD(Grand Central Dispatch)의 개념을 이해하고, 사용하고 있다. 설명해보세요.	"- 장희 : GCD는 애플에서 쓰레드를 관리하기 위해 만든 기술로 작업별로 블록을 만들어서 사용할수 있는 FIFO 형태의 Queue를 제공해 주는 것을 말합니다. 실제로 사용 할때는 
DispatchQueue 형태로 사용하게 됩니다. DispatchQueue는 serial 과 Concurrent로 나누어집니다. serial은 블록이 직렬로 실행되는것을 말하고 concurrent는 병렬로 실행되는것
을 말합니다. 또 동기와 비동기로 작업을 하게 할수도 있습니다. 동기는 작업을 요청하면 작업이 종료 될대까지 기다리는것을 말하고, 비동기는 우선 메서드를 종료하고 결과는 후에 받는 
걸로 알고 있습니다. 특별히 사용한 계기를 설명하기는 어렵지만 UI관련된 작업은 교착상태 때문에 serial로 실행되는 main의 경우 비동기로 작업을 해줘야 했고 그렇게 하지 않으면 메
모리 관련 에라가 컴파일 단계에서 발생했던걸로 기억합니다."									
화면이 멈추지 않게 하려면 어떤 스레드를 건드리지 말아야 하는지 알고 있다. 설명해보세요.	"- 장희 : 화면이 멈추지 않게 하려면 메인쓰레드를 건드리지 않아야 하는걸로 알고 있습니다. 어플리케이션이 실행되면 메인쓰레드가 부여 되는데 그 쓰레드에서 통신 작업과 같이
비동기로 해야 하는 작업을 하면 그 통신의 결과를 기다리는 동안 UI가 표현되지 않아 사용자는 화면이 멈춰 있는다고 느끼게 될것 같습니다."									
- Background Task를 이용해 백그라운드에서 동작하는 작업을 만들어 보았다. 설명해보세요.	안만들어봤습니다.									
- AppDelegate에서 앱의 상태변화에 따라 호출되는 함수에 대해 명확히 알고 있다. 설명해보세요.	"application(_:didFinishLaunching:) - 앱이 처음 시작될 때 실행
applicationWillResignActive: - 앱이 active 에서 inactive로 이동될 때 실행 
applicationDidEnterBackground: - 앱이 background 상태일 때 실행 
applicationWillEnterForeground: - 앱이 background에서 foreground로 이동 될때 실행 (아직 foreground에서 실행중이진 않음)
applicationDidBecomeActive: - 앱이 active상태가 되어 실행 중일 때
applicationWillTerminate: - 앱이 종료될 때 실행"									
UIViewController의 Life Cycle에 대해 명확히 알고 있다. 설명해보세요.	"- 장희 : init -> viewDidLoad -> viewWillappear -> viewDidappear -> viewWillDisappear -> viewDidDispaaer
초기화 -> 메모리에 뷰컨트롤러가 올라 간다음 -> 뷰컨트롤러가 보이기 전 -> 뷰컨트롤러가 보이고 난 후 -> 뷰컨트롤러가 메모리에서 제거 되기 전 -> 뷰컨트롤러가 메모리에서 제거 된 후"									
- CustomScheme를 이용해 딥링크 기능을 구현한 경험이 있다. 설명해보세요.	- 장희 : 페이스북 관련 화이트리스트를 등록해서 구현해본것 같다 (자세하게는 모르겠네.. 기억이 안나.. 다시 해봐야 해요)									
- Universal Link를 사용해 웹에서 앱을 연동한 경험이 있다. 설명해보세요.	- 장희 : OPENURLScheme 를 말하는것 같음, 셋팅 화면으로 이동하고 그런거 구현해 본걸 다시 살펴 보면 될듯									
- Google Analytics, Tune, Fabric등 모바일 애널리틱스 툴을 연동한 경험이 있다. 설명해보세요.	안해봤습니다.									
- Push 서비스를 구현한 경험이 있다. 설명해보세요.	이거우리수업시간에한건가요									
인터넷이 느리고 불안정한 지역에서 서버로 API를 호출하여 10만 개의 데이터를 리스트로 보여줘야 합니다. 이 문제를 해결하는 과정 및 그 과정 중에 구현할 요소들과 단계별 고려사항들을 설명해주세요.	잘모르겠습니다.									
- UICollectionView와 UITableView의 스크롤 속도를 최적화를 위해 어떠한 방법을 사용해보셨나요? 설명해보세요.	"뜽진 : SDWebImage(옵잭씨), Kingfisher(Swift)등의 이미지 캐싱처리 라이브러리를 사용하면 비동기적으로 동작하기때문에 좀 더 자연스러운 스크롤이 가능하고,
Cell들을 재사용하는 작업을 진행중에 본래 라이브러리들도 DisqatchQueue.main.async를 이용해 작업을 하고있어 좀 더 빠른 스크롤이 가능합니다."									
- 선호하는 UI 구현 방식에 대해 설명해주세요.	이섭: - MVVM ( 테스트용이성, 왜냐면 뷰모델에서는 UIKit관련된 코드가 없기때문에 UI만 독립적으로 테스트할수있다. WWDC애서는 의존성주입을 사용하라고 권장했는데 제생각은 너무 많은 의존성이 포함된 뷰컨트롤러 코드는 가독성이 떨어지는거 같다 . 그리고 코드파악도 힘들다. ) 									
- iPhone의 다양한 해상도를 지원하기 위해 어떤 방식을 활용하고 있는지, 다양한 해상도를 지원하기 위해 특별히 고려한 것들이 있는지 설명해주세요.	"단말에 대한 분기처리를 하기 보단 오토레이아웃을 이용하여 전체 단말을 통합하는 UI를 만들려고하고 있습니다.
사이즈 클래스를 이용해서 한 스토리보드 화면에 iPad, iPhone 등을 나눠서 작업 할 수 있습니다."									
- 자주 사용하는 오픈소스는 어떤 것들이 있나요? 그 오픈소스를 선택한 이유는 어떤건가요? (가급적이면 AFNetworking과 SDWebImage 이외의 것들을 소개해주세요.)
Toaster (간단한 인터페이스 같은 토스 , 알림창띄우기보단 사용법이 간단하 자주 사용하고있습니다.)
ObjectMapper (모델 객체 (클래스 및 구조체)를 JSON으로 쉽게 변환 할 수있게 해주는 Swift로 작성된 프레임 워크)
Then (간단하게 swift initializers)
Alramofire, Kingfisher"	

- 참여한 오픈소스가 있나요?  설명해보세요.								
										
