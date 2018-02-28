
### 생성, 실행

프로젝트를 생성합니다
vue init webpack-simple (디렉토리 이름)

디렉토리 이름이 생략될 경우 다음은 질문합니다
Generate project in current directory? **01**

그리고 연달아 질문이 나타납니다
Project name **vue-cli**
Project description **vue-cli**
Author **Jun-mo <yunedoopea610@gmail.com>**
License **MIT**
Use sass? **No**

모듈을 다운받습니다
npm install

그리고 실행 하세요
npm run dev

브라우저를 열어 접속하세요
localhost:8080

### 디렉터리 구조
- node_modules: 모듈이 다운되는 곳(npm install)
- src: 웹 어플리케이션이 만들어지는데 필요한 자료
  - assets: 자원(이미지, 동영상)
- index.html: 웹 앱의 시작점. npm run dev 실행 시 로딩되는 파일
- package.json: npm 설정 파일. 의존성을 정의하는 파일
- webpack.config.js: 웹팩 설정 파일. 웹팩 빌드를 위해 필요한 로직들을 정의하는 파일