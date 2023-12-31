# Foundation과 Library의 차이점
**해당 글은 공부를 하며 지속적으로 업데이트 할 예정입니다.*
<br/><br/>
예전부터 라이브러리와 프레임워크에 대한 차이점을 이해하려고 많이 노력했다.<br/>
그럼에도 불구하고 쉽게 이해할 수 없었는데, '제어의 주도권이 바뀐다'는 점이 덜 이해되서 그랬던 것 같다.<br/><br/>
여전히 이해가 되지 않지만, 가만히 있으면 그저 흘러 보낼 것 같아서 정리를 해보고자 한다.
<br/><br/>
### 1. 라이브러리(Library)
**개인적으로 라이브러리는 말 그대로 도서관 같은 개념이다.**<br/>
예전에는 우리가 궁금한게 있으면 많은 선택지 중에 도서관을 가서 책을 읽었다.<br/>
그 이유는 내가 궁금해 하는 분야에 대한 책들이 한 곳에 몰려 있는 section들을 찾을 수 있고 정보를 찾을 수 있기 때문인데, 코드도 비슷하다. 라이브러리에는 메서드 또는 역할 등에 따라 코드들이 묶여 있다.<br/> 이 코드들을 일일히 반복해서 작성할 필요없이 그저 작성하기만 하면 사용이 가능하다!
<br/><br/> 많은 예시들은 자동차를 빗대어 라이브러리는 핸들이다, 휠이다 등등 설명을 해주고 있는데,<br/> 차에 관심이 없어서인지 이해가 항상 안 갔다.<br/> 
거대한 한 조직의 한 역할을 맡는 부품들 자체를 라이브러리로써 보는 건지,<br/>
굴러가는 차량의 주요 역할을 담당하는 핸들과 휠이기에 라이브러리인지 등이 이해가 안됐다.

적어도 지금 느끼기로는 후자가 아닐까 싶다.
모든 코드 단위를 라이브러리로 보기보다 어떤 책임과 역할을 맡은 코드들의 묶음을 라이브러기가 아닐까 생각한다. 더불어 라이브러리는 개발자가 호출하는 형태를 가졌다.
<br/><br/>
### 2. 프레임워크(Framework)
그렇다면 프레임워크는 뭘까?<br/>
**기본적으로 이해하고 있는건 라이브러리는 프레임워크 내에 속한다.**

이유는 프레임워크는 이름에서 추측할 수 있다시피, Frame(뼈대)를 의미하고 있다.<br/>
우리가 문법을 배울 때 모든 코드를 하나하나 다 외우면서 공부를 하지 않듯이, 어플을 구현할 때도 라이브러리에 있는 코드를 다 외워서 적재적소에 코드를 넣지 않는다. 아니 못한다 생각한다. <br/>
그 이유는 너무 방대해서!

고로, 프레임워크는 특정 역할을 담당하는 코드들과 라이브러리들이 묶인 코드를 의미하나<br/>
역할보다 좀 더 큰 개념인, 어떤 서비스 또는 기능을 제공하기 위한 단위로 이해했다. 
<br/><br/> 추가적으로 찾은 정보에서는 프레임워크는 구현하기 위해서 일종의 규칙과 제약이 많은 라이브러리라고 한다. <br/> 특정 규칙을 따라야지만 우리가 원하는 기능이나 서비스를 구현할 수 있는 구성이 프레임워크라 한다.



### 3. 주도권이란 무엇인가


### 참고
- https://www.devkuma.com/docs/framework-and-library/<br/>
좋은 링크를 공유해준 현빈 팀원에게 무한한 감사!
- https://hackr.io/blog/what-is-frameworks#what-is-a-framework
- https://www.youtube.com/watch?v=t9ccIykXTCM