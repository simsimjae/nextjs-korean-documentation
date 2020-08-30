# Next.js 9.5.2 공식문서 한글판

이 문서는 저자가 Next.js의 공식문서를 보고 번역, 의역, 해석한 내용이므로 정확히 일치하지 않을 수 있습니다.
또한 너무 쉬운 내용은 적지 않았으니 빠진 내용은 공식문서를 참고해주세요.

## Update History

- 1차 버전 : 2020.08.30 ~

# 설치

```bash
npx create-next-app
# 또는
yarn create next-app
```

# 수동 설치

```bash
npm install next react react-dom
```

package.json 열어서 다음 스크립트 추가

```bash
"scripts": {
  "dev": "next dev",
  "build": "next build",
  "start": "next start"
}
```

- `dev`: Next.js 개발 모드로 실행
- `build`: production용으로 Next.js 빌드
- `start`: production용으로 Next.js 실행

Next.js는 `pages`폴더 아래에 있는 `.js, .jsx, .ts, .tsx`파일들로부터 export된 리액트 컴포넌트를 페이지로 인식한다.
Pages아래에 있는 컴포넌트들은 파일의 이름을 기반으로 라우팅 된다. 예를들어 `pages/about.js`는 `/about`으로 라우팅하여 접근할 수 있다.

## 더 알아둬야 할 것

- Next.js는 내부적으로 웹팩과 바벨을 사용한다.
