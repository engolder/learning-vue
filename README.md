<p align="center"><a href="https://vuejs.org" target="_blank"><img width="100" src="https://vuejs.org/images/logo.png" alt="Vue logo"></a></p>

_로고 클릭시 Vue js 공식 문서로 이동합니다_

# learning Vue

프로젝트에 사용하기 위한 vue.js 를 공부한 기록이 정리된 레포지토리입니다.

### Vue.js 내용 정리

* **Vue.js**: 사용자 인터페이스를 개발하기 위한 javascript 프레임워크
* Vue.js 특징:
  * **복잡성**: 타 프레임워크와 비교하여 프로젝트에 사용하기 위한 필요 학습 기간이 많지 않다.
  * **데이터 바인딩**: 컴포넌트 간 단방향 데이터 흐름
  * **작은 규모**
  * **단일파일 컴포넌트**:
    * HTML 과 CSS, JS 를 포함한 하나의 .vue 파일
    * 컴포넌트 내부는 랭귀지 블럭으로 이루어져있다.
    * 템플릿 블럭, 스타일 블럭, 스크립트 블럭
  * **한글 지원 공식 가이드**: 이 문서만으로 웹 어플리케이션을 제작할 수 있다. <https://kr.vuejs.org/v2/guide/>
* Vue.js 설치:
  * **vue-devtool**: 브라우저를 위한 디버거 <https://github.com/vuejs/vue-devtools#vue-devtools>
  * Standalone: JavaScript 파일을 HTML 의 script 태그를 통해 불러오는 것
    * **개발용 버전**: <https://vuejs.org/js/vue.js>
    * 배포용 버전: <https://vuejs.org/js/vue.min.js>
  * NPM:
    * \# 최신 안정화 버전
    * **$ npm install vue**
  * CLI:
    * \# vue-cli 설치
    * **$ npm install --global vue-cli**
    * \# "webpack" 템플릿을 이용해서 새 프로젝트 생성
    * **$ vue init webpack my-project**
    * \# 의존성을 설치하고 실행하세요!
    * **$ cd my-project**
    * **$ npm install**
    * **$ npm run dev**
  * Bower:
    * **$ bower install vue**

### 용어 정리

* MVVM 패턴(Model-View-ViewModel): 마크업 언어나 GUI코드를 비즈니스 로직 또는 백엔드 로직과 분리하여 개발하는 소프트웨어 디자인 패턴
* 뷰(view): 사용자에게 보이는 화면
* 돔(DOM): HTML 문서에 들어가는 요소의 정보를 담고 있는 데이터 트리
* 돔 리스너(DOM Listener): 돔의 변경 내역에 대해 즉각적으로 반응하여 특정 로직을 수행하는 장치
* 모델(Model): 데이터를 담는 용기. 보통은 서버에서 가져온 데이터를 자바스크립트 객체형태로 저장
* 데이터 바인딩(Data Binding): 뷰에 표시되는 내용과 모델의 데이터를 동기화
* 뷰 모델(ViewModel): 뷰와 모델의 중간 영역. 돔 리스너와 데이터 바인딩을 제공하는 영역
* 라우팅(Routing): 웹 페이지 간의 이동 방법
* SPA(Single Page Application): 페이지를 이동 시에 클라이언트의 라우팅을 이용하여 화면을 갱신하는 패턴을 적용한 애플리케이션
* 라우터(View Router): 라우팅 기능을 구현할 수 있도록 지원하는 라이브러리
* 네스티드 라우터(Nested Router):
* 네임드 뷰(Named View):
* 프로토콜(Protocol): 컴퓨터나 단말기 간에 통신하기 위해 상호간에 정의한 규칙
* ajax: 서버에서 받아온 데이터 표시 때 화면의 일부분만 변경할 수 있게 하는 제이쿼리의 자바스크립트 기법
* 뷰 리소스(View Resource): 뷰에서 ajax를 지원하기 위해 제공하는 라이브러리
* axios: 뷰 커뮤니티에서 가장 많이 사용되는 HTTP통신 라이브러리
* 컴포넌트(Component): 조합하여 화면을 만드는 단위, 레고 블럭을 생각하면 쉽다
* 렌더링(rendering): 템플릿 문법을 해석하여 HTML 로 변환되는 과정
* 훅(hook): 특정 지점에서 일어나는 동작
* 래퍼(wrapper): template 와 같이 요소들을 묶어주는 역할
* 버블링(bubbling): 이벤트가 자식 엘리먼트 쪽으로 전파되는 것
* 캡처링(capturing): 이벤트가 부모 엘리먼트 쪽으로 전파되는 것
* 체이닝(chaining): 명령어를 잇다라 적는 방식
* 모듈 번들러(Module Bundler): 서로 의존 관계가 있는 모듈을 하나의 파일로 묶어 주는 도구 

### Vue.js 참고 문헌

* vue.js gihub <https://github.com/vuejs/vue>
* vue.js 한국 사용자 모임 <https://vuejs-kr.github.io/>
* vue.js 한글 문서 <https://kr.vuejs.org/v2/guide/>
* Vue.js 이 정도는 알아야지 - Tour of Vue.js : 김지환 | 이선협
* 쉽고 빠르게 배우는 Vue.js2 프로그래밍 : 알렉스 키리아키디스 | 코스타스 매니아티스
* Do it! Vue.js 입문 : 장기효
