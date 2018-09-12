# interviewpc


- 아이폰 개발 시작동기와 학습 방법
프로그래밍을 해보자고 생각했을때 하드웨어가 완성되어 있는 상태면 좋겠다는 생각을 했었습니다. 그걸 사용해서 하드웨어의 특징을 살려서 좋은 기능을 구현해 볼수도 있을것 같았고 지금 만들어져있는 어플들을 많이 사용하고 있는데 이 경험을 살려 더 좋은 서비스를 만들어 낼수 있을것 같다는 생각이 들어서 아이폰 개발을 시작하게 되었습니다.

- 주로 사용하는 패턴이나 좋아하는 개발 방법론과 그 이유
지금은 MVC 패턴을 사용하려고 노력하고 있습니다. 이유는 Swift에서 기본적으로 알아야 되는 패턴이라고 생각이 들어서입니다. 지금 관심이 있는 패턴은 MVVM인데 공부를 제대로 해서 실제로 사용을 해보고 싶습니다. 개발 방법론은 개인적으로는 페어프로그래밍에 대해서 관심이 좀 있습니다. 페어프로그래밍은 한 컴퓨터를 2명의 사용자가 사용하는 방식으로 알고 있는데 개발을 진행하면서 프로젝트를 하다보면 이게 최선인지 찝찝한 느낌이 드는 부분들이 있을것 같은데 그때 바로바로 이야기 하면서 해결을 빨리 할수 있을것 같고 개인적으로 가지고 있을수도 있는 나쁜 습관들을 고칠수 있을수도 있다고 생각하기 때문입니다.

- Hybrid 앱 개발 경험이 있는가  ?
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

- 정수를 입력받아 입력받은 수에 해당하는 자리의 피보나치 숫자를 반환하는 함수
피보나치 수열이란 앞의 두 수를 더하면 뒤의 수

