## 분리한 컴포넌트 목록
- /src/components
  - Button
  - Input
  - Title
  - List
- /src/assinment/01
  - TodoItem
  - TodoList

## ❓ Why: 과제 제출시에는 아래 질문의 답변과 함께 제출해주세요.
#### Q1. JSX 문법이란 무엇일까요?
: html/xml과 유사하게 생긴, javascript 기반 문법이다.
브라우저가 해석할 수 없어 babel과 같은 툴을 이용해 변환해 브라우저에게 넘겨야 한다.

#### Q2. 사용자가 입력하는 값, 또는 이미 입력된 값, 투두의 타이틀과 같은 애플리케이션의 상태를 관리하기 위해 리액트의 어떤 기능을 사용하셨나요?
: useState를 사용했다. useState는 컴포넌트의 상태 관리해주는 Hook으로, 값이 변경될 때마다 화면을 리렌더링하는 기능을 제공한다.

#### Q3. 애플리케이션의 상태 값들을 컴포넌트 간 어떤 방식으로 공유하셨나요?
: 부모 state를 자식 컴포넌트의 props로 넘겨주었다. state와 달리 state를 변경하는 setter 함수는 랩핑한 콜백함수로 만들어 props로 넘겨주었다.

#### Q4. 기능 구현을 위해 불변성 유지가 필요한 부분이 있었다면 하나만 설명해 주세요.
: 잘 모르겠다. 다만, 가변 데이터의 트래킹은 어렵기에 쉽게 오류를 낳는다. 꼭 필요한 변경 외에는 기본적으로는 불변성을 유지해주는 게 좋다.

#### Q5. 반복되는 컴포넌트를 파악하고 재사용할 수 있는 컴포넌트로 분리해 보셨나요? 그렇다면 어떠한 이점이 있었나요?
: 재사용성과 수정 용이성에 좋았다.
