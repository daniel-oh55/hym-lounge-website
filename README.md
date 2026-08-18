# HYM LOUNGE Website

HYM LOUNGE 공식 조직 웹사이트와 모바일 애플리케이션 소개 페이지입니다. 별도의 빌드 과정 없이 정적 HTML과 CSS만으로 구성되어, GitHub `main` 브랜치가 Vercel에서 그대로 배포될 수 있도록 설계되었습니다.

## 운영 도메인

- https://hymlounge.com
- https://www.hymlounge.com

`hymlounge.com`은 Vercel 설정을 통해 `www.hymlounge.com`으로 리다이렉트됩니다.

## 페이지 구조

```text
/
├─ index.html
├─ styles.css
├─ 404.html
├─ robots.txt
├─ sitemap.xml
├─ assets/
│  └─ favicon.svg
├─ harupuli/
│  ├─ index.html
│  ├─ privacy/
│  │  └─ index.html
│  └─ terms/
│     └─ index.html
├─ minmove/
│  └─ privacy/
│     └─ index.html
└─ support/
   └─ index.html
```

## 사용 기술

- HTML5
- CSS3
- 시스템 폰트
- 외부 UI 프레임워크, CDN 폰트, 외부 이미지, npm 패키지 없음

## 로컬 실행

저장소 루트에서 정적 서버를 실행합니다.

```bash
python -m http.server 4173
```

브라우저에서 다음 주소로 접속합니다.

```text
http://localhost:4173
```

## 배포

Vercel은 GitHub `main` 브랜치를 기준으로 자동 배포합니다. Pull Request를 `main`에 병합하면 운영 도메인에 정적 파일이 반영됩니다.

## 출시 전 확인 사항

하루풀이 개인정보처리방침의 광고 및 분석 SDK 관련 내용은 앱의 실제 구현과 일치해야 합니다. Google AdMob, Firebase Analytics, Crashlytics 또는 기타 광고·분석 SDK 도입 여부가 확정되면 출시 전에 개인정보처리방침과 Google Play 데이터 보안 정보를 다시 검토해 주세요.
