# MVVM

역할과 책임으로 코드를 분리하는데, 일반적으로 네트워크 관련 코드들은 singleton으로 작성을 한다. > *이유는?

*다양한 클래스에서 어차피 같은 역할을 하는 친구를 참조하고 있다면 굳이 여러개 만들어서 할 필요가 없다는 점이다. Singleton으로 하나만 생성하고 처리를 하면 된다는 점인데 이것도 의존성 분리를 할 수 있는 하나의 방법인 셈


결국 모든 아키텍쳐는 코드를 분리하기 위함
*Architecture이라고 할 때 대부분 만들어가는 구조임에도 불구하고 분리를 한다는 점이 웃기다.*

MVC의 대체안으로 MVVM이 언급되지만 실질적으로 MVVM도 비대해지는 경우가 있다고 한다.
이때 Viper, TCA 등을 도입한다고 하는데, 이건 해보면서 경험해보자.


올바른 아키텍쳐의 선택 기준은 유지보수에 용이해야하기 때문
명확한 분리 기준은 단일 책임 원칙을 따르며
테스트 가능은 TDD 와 유닛 테스트가 가능해야 더 안전한 코드 작성으로 가능해진다.

viewModel은 NSObject로 UIKit를 import하지 않기에 기존 UI에 변화를 주는 형식으로 코드를 작성하지 않아도 된다.



간단하게 보면 View는 viewController와 view를 합친 구조가 된다.
model은 기존 데이터 모델 그대로 유지를 하는데,
해당 모델의 데이터를 담게 되는 그릇이 viewModel로 모델을 가지면서 동시에 해당 데이터에 변동을 주는 메서드 (로직) 등을 가지게 된다.

*viewController의 책임감 무게를 덜어가는 시스템*