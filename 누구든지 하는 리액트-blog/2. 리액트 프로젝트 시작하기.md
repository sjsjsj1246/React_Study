# 리액트 프로젝트 시작하기

- 리액트 프로젝트는 jQuery같은 것을 단순히 <script src="..."></script> 의 형태로 불러와서 사용했던 것 처럼 사용하지 않는다. 그대신 Node, yarn, Webpack, Babel등의 도구를 설치하여 프로젝트를 설정해주여야 한다.
- 리액트 프로젝트를 바닥부터 설정하는 것은 초심자에게는 꽤나 복잡한 작업이나, 페이스북에서 제공해주는 [create-react-app](https://github.com/facebook/create-react-app)을 통하여 이 작업을 간단하게 준비해줄 수 있다.

## Webpack, Babel은 무슨 용도인가?

- 리액트 프로젝트를 만들게 되면서, 컴포넌트를 여러가지 파일로 분리해서 저장 할 것이고, 또 이컴포넌트는 일반 자바스크립트가 아닌 JSX라는 문법으로 작성하게 됩니다.
- 여러가지의 파일을 한개로 결합하기 위해서 Webpack이라는 도구를 사용하고, JSX를 비롯한 새로운 자바스크립트 문법들을 사용하기 위해서 Babel이라는 도구를 사용한다.

## 개발환경 구축법

- node.js 설치 : https://nodejs.org/ko/download/
    Webpack과 Babel같은 도구들이 자바스크립트 런타임인 Node.js를 기반으로 만들어져 있다.
- Yarn 설치 : https://yarnpkg.com/en/docs/install
    - node.js 의 패키지 매니저인 npm의 상위호환 버전이다.
    - 프로젝트에 사용되는 라이브러리를 설치하고 해당 라이브러리들의 버전 관리를 하게 될 때 유용하다. 
- create-react-app 설치 및 사용:
    - 터미널에서 yarn global add create-react-app 하면 설치완료
    - 원하는 위치에서 create-react-app hello-react 프로젝트 생성
    - cd hello-react 로 해당 프로젝트로 이동
    - yarn start 로 시작