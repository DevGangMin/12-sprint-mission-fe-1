🐼 판다마켓 (Pandamarket)

일상의 모든 물건을 거래하는 중고 거래 플랫폼 랜딩 페이지
HTML, CSS 기반 정적 웹 프로젝트

📌 프로젝트 소개

판다마켓은 중고 물품을 쉽고 안전하게 거래할 수 있는 플랫폼을 목표로 제작된 웹 페이지입니다.
HTML + CSS만으로 구현하였습니다.

🛠️ 기술 스택

HTML5

CSS3

Netlify 

Google Analytics 4 

📂 프로젝트 구조
pandamarket/
├── index.html
├── login.html
├── signup.html
├── items.html
├── privacy.html
├── faq.html
├── css/
│   ├── reset.css
│   ├── style.css
│   ├── login.css
│   └── signup.css
└── images/
    ├── index/
    ├── login/
    └── signup/

📄 페이지 구성

1️⃣ 랜딩 페이지 (/)

GNB (로고, 로그인 버튼)

HERO 섹션

인기 상품 소개

상품 검색 안내

상품 등록 안내

Footer (Privacy / FAQ / SNS 링크)

2️⃣ 로그인 페이지 (/login)

이메일 입력

비밀번호 입력

간편 로그인 (Google / Kakao)

회원가입 이동 링크

3️⃣ 회원가입 페이지 (/signup)

이메일

닉네임

비밀번호

비밀번호 확인

간편 로그인

🎨 CSS 설계 방식

1️⃣ CSS 변수 활용

Palette에 정의된 색상값을 :root에 CSS 변수로 등록하여 사용하였습니다.

:root {
  --primary: #3692ff;
  --text: #111827;
  --muted: #6b7280;
  --input-bg: #f3f4f6;
  --social-bg: #e6f2ff;
}

→ 유지보수성과 재사용성을 높이기 위한 설계입니다.

2️⃣ Flexbox 기반 레이아웃

display: flex

justify-content

align-items

gap

을 활용하여 반응형에 유연한 구조를 설계하였습니다.

3️⃣ 시맨틱 태그 사용

<main>

<section>

<nav>

<footer>

를 사용하여 웹 접근성과 구조적 의미를 고려하였습니다.

📊 Google Analytics 설정

방문자 수 확인을 위해 **GA4 (Google Analytics 4)**를 연동하였습니다.

<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>

실시간 보고서에서 방문자 확인 가능

🚀 배포

Netlify를 통해 배포 

루트 경로(/)를 랜딩 페이지로 설정

✨ 주요 구현 포인트

UI 라이브러리 없이 순수 HTML/CSS로 구현

CSS 변수로 색상 통합 관리

버튼 및 링크에 cursor: pointer 적용

간편 로그인 아이콘 정렬 개선

shrink 방지 설계

접근성을 고려한 aria-label 사용

👩‍💻 제작자

정민