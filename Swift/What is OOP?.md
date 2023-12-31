# 230726 OOP는 좋은 프로그래밍 방식일까?
매우 얕은 공부를 하며 OOP에 대한 생각을 정리하고 업데이트 해보고자 한다!

## TIGO(Today I Go Over)
### OOP는 무엇일까?

Object-Oriented Programming의 줄임말로, 객체 지향 프로그래밍이라고 불린다. Alan Kay라는 사람이 만들었다시피 불리는 이 프로그래밍 패러다임/방식은 완벽하게 분리된 서로 다른 객체들이 정보 교환(메시징)을 통해 임무를 완성 시킨다.<br/><br/> 간단 예시를 들면, 사람이 자판기에서 커피를 뽑아내려고 한다고 가정하자.
커피를 뽑기 위해 사람은 ❶ 지갑을 꺼내 돈을 확인하고 ❷ 자판기 금액을 확인하고 ❸ 알맞는 금액을 자판기에 넣어 원하는 음료를 선택할 것이다. 이때 자판기는 ❹ 받은 돈이 음료 금액과 크거나 같은지 확인하고 ❺ 음료를 사람이 받을 수 있도록 출구로 보낼 것이다.
<br/><br/>**이 상황만으로 OOP가 설명됐다!**<br/>
여기서 사람과 자판기는 Object(객체)다.<br/>
객체들은 서로 무엇을 가지고 있는지는 모른다. (디스플레이처럼 보여주는 무언가가 있지 않는 이상)<br/>사람은 본인이 가진 돈을 확인하고 금액만 넣었을 뿐, 실제로 커피를 만드는 행동은 자판기에서 한다. 이게 바로 객체 지향 프로그래밍이 지향하는 방향이다. 사람은 '커피'라는 결과물만을 원할 뿐, 자판기가 어떻게 만드는지는 신경을  쓰지 않는다.<br/><br/>


## 그래서 OOP가 좋은걸까?
이미 OOP는 여러 프로그램에서 이미 그의 시선을 따르고 있다.<br/>Java, Python, C++ 등은 이 패러다임을 일부 채택해서 따라가고 있다고 하는데, OOP가 어떤 점에서 좋고 왜 따르는지 궁금해졌다.
<br/>

코딩은 구현, 효율성 등등 챙겨야할 게 많은 것 같다.<br/>
하지만 다양한 패러다임들이 등장한 이유는 **지저분한 코드** 때문에 나타난게 아닐까 싶다. Spaghetti code라고 부르는 현상을 방지하고 벗어나고자 프로토콜 지향적, 객체 지향적, 함수형 등등 다양한 관점에서 좋다고 생각되는 프로그래밍 방식이 등장한 것으로 이해하고 있는데, OOP는 책임과 담당 역할에 따라 분리가 된다는 점에서 좋게 판단되는 프로그래밍 방식이 아닐까 싶다.

더불어서 궁극적인 목표 중 하나가 결국 코드를 줄여 반복되는 repetition을 없애기 위한게 아닐까?
<br/><br/>
## 그럼에도 '무조건' OOP가 좋다는 의미는 아니다.
개인적으로 느끼는 것도 개발을 처음하는 입장에서 '실세계를 구현한 듯한 프로그래밍 방식'이라고 해서 이론적인 접근이 가깝게 다가왔을 뿐이지, 실제로 코드를 짜보면 물음표를 많이 던지게 된다.

클래스가 제공하는 상속만 바라봐도 애매해지는 경우가 많다.<br/>
단일 상속만 지원하는 클래스에 굳이 상속이라는 기능이 왜 필요한 걸까. 작성해야하는 코드를 줄여 주기는 하지만, 상속을 활용하고자 할 때, 혹은 갑자기 추가를 해야할 때, Parent Class가 지녀야하는 프로퍼티와 메서드에 대한 고민이 정말 많아져야 한다는 생각을 한다.