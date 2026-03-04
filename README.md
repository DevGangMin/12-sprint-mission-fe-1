# 🐼 판다마켓 프로젝트

스프린트 미션 part1 레포지토리입니다.

> 배포 링크: https://12-sprint-mission-yooseohyeon.netlify.app

## 📁 프로젝트 구조

```
...
├── index.html
├── login.html
├── signup.html
├── .gitignore
├── css/
│   ├── reset.css      # 브라우저 기본 스타일 초기화
│   ├── common.css     # 공통 변수·타이포그래피·버튼 스타일
│   ├── index.css      # 메인 페이지 전용 스타일
│   └── auth.css       # 로그인/회원가입 공통 스타일
├── images/
│   └── (이미지·아이콘 파일)
└── README.md
```

## ✨ 주요 기능

- **메인 페이지**: 서비스 소개, 로그인 페이지 이동
- **로그인 페이지**: 이메일/비밀번호 입력, 소셜 로그인(Google, Kakao)
- **회원가입 페이지**: 이메일, 닉네임, 비밀번호 입력, 소셜 로그인

## 🎨 주요 구현 사항

### CSS 아키텍처

- **스타일 레이어 분리**: `reset` → `common` → 페이지별 스타일 순으로 분리
- **공통 컴포넌트 스타일**: `:root`에 색상 토큰 정의, 타이포그래피·버튼을 재사용 가능한 클래스로 관리
- **BEM 네이밍**:`.auth__container`, `.auth-form__input`등 Block-Element-Modifier 규칙 적용
- **로그인·회원가입 스타일 통합**: 두 페이지의 구조가 유사하므로 `auth.css` 하나로 통합하고, 차이가 있는 부분만 `.auth--signup` 같은 modifier로 분기해 중복 최소화

### 접근성

- 시맨틱 태그(`<header>`, `<main>`, `<footer>`, `<section>`, `<nav>`) 사용
- `sr-only` 클래스로 스크린 리더 전용 텍스트 제공 (비밀번호 보기 버튼, 폼 legend, sns 링크 등)
- 장식용 이미지에 `alt=""`, `aria-hidden="true"` 처리

---

본 프로젝트는 코드잇의 소유이며, 교육 목적으로만 사용됩니다. © 2025 Codeit. All rights reserved.
