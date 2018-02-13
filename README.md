# learning Vue
- vue.js gihub https://github.com/vuejs/vue
- vue.js 한국 사용자 모임 https://vuejs-kr.github.io/
- vue.js 한글 문서 https://kr.vuejs.org/v2/guide/


<svg height="150" viewBox="0 0 256 221" preserveAspectRatio="xMinYMin meet"><path d="M204.8 0H256L128 220.8 0 0h97.92L128 51.2 157.44 0h47.36z" fill="#41B883"/><path d="M0 0l128 220.8L256 0h-51.2L128 132.48 50.56 0H0z" fill="#41B883"/><path d="M50.56 0L128 133.12 204.8 0h-47.36L128 51.2 97.92 0H50.56z" fill="#35495E"/></svg>
## Vue.js
- 사용자 인터페이스를 만들기 위한 진보적인 프레임워크
- 다른 단일형 프레임워크와 달리 Vue는 점진적으로 채택할 수 있도록 설계됨
- 핵심 라이브러리는 뷰 레이어만 초점을 맞추어 다른 라이브러리나 기존 프로젝트와의 통합이 용이함

### 뷰 사용
    - 뷰 다운로드 및 경로지정 : https://vuejs.org/
    - unpkg에서 제공하는 링크 : <script src="https://unpkg.com/vue/dist/vue.js"></script>
    - 혹은 : https://jsfiddle.net/chrisvfritz/50wL7mdz/

## Vue 시작
------
### 간단한 템플릿 구문을 사용해 선언적으로 DOM에 데이터를 렌더링
    <div id="app">
        {{ message }}
    </div>