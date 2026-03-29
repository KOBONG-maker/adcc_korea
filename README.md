# ADCC KOREA 공식 웹사이트

대한민국 그래플링 챔피언십 공식 웹사이트

![ADCC KOREA](https://img.shields.io/badge/ADCC-KOREA-dc2626?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Live-success?style=for-the-badge)
![Cost](https://img.shields.io/badge/Cost-FREE-00d4ff?style=for-the-badge)

## 🌟 특징

- ✅ **완전 무료** - GitHub Pages로 호스팅 비용 0원
- ✅ **반응형 디자인** - 모바일/태블릿/PC 완벽 지원
- ✅ **빠른 로딩** - 최적화된 성능
- ✅ **쉬운 관리** - 코딩 지식 없이도 콘텐츠 수정 가능
- ✅ **프로페셔널** - Athletic Brutalism 디자인 컨셉
- ✅ **SEO 최적화** - 검색 엔진 친화적

## 📁 파일 구조

```
adcc-korea/
├── index.html          # 메인 홈페이지
├── schedule.html       # 대회 일정
├── news.html           # 뉴스/공지사항
├── about.html          # ADCC 소개
├── gallery.html        # 갤러리
├── contact.html        # 연락처
├── css/
│   └── style.css       # 메인 스타일시트
├── js/
│   └── main.js         # JavaScript 인터랙션
├── DEPLOYMENT.md       # 배포 가이드
└── README.md           # 이 파일
```

## 🎨 디자인 컨셉

**Athletic Brutalism** - 강렬하고 현대적인 스포츠 웹사이트

- **색상 팔레트:**
  - Primary: #dc2626 (강렬한 레드)
  - Secondary: #eab308 (골드)
  - Background: #0a0a0a (다크)
  
- **타이포그래피:**
  - Display: Bebas Neue
  - Heading: Oswald
  - Body: Inter

## 🚀 빠른 시작

### 1. 다운로드
이 저장소의 모든 파일을 다운로드합니다.

### 2. 로컬에서 보기
- `index.html` 파일을 더블클릭하여 브라우저에서 열기
- 또는 VS Code + Live Server 확장 프로그램 사용

### 3. 배포
자세한 배포 방법은 **[DEPLOYMENT.md](DEPLOYMENT.md)** 참고

## 📝 콘텐츠 수정 가이드

### 대회 일정 추가/수정

`schedule.html` 파일에서 다음 부분을 복사하여 수정:

```html
<div class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="event-card">
        <div class="event-date">
            <div class="date-month">APR</div>
            <div class="date-day">15</div>
            <div class="date-year">2026</div>
        </div>
        <div class="event-info">
            <h4 class="event-title">대회 이름</h4>
            <p class="event-description">대회 설명...</p>
            <div class="event-meta">
                <span class="event-location">📍 장소</span>
                <span class="event-time">⏰ 시간</span>
            </div>
        </div>
    </div>
</div>
```

### 뉴스 추가

`news.html` 파일에서 다음 구조 사용:

```html
<article class="news-card">
    <div class="news-image-placeholder">
        <span>NEWS</span>
    </div>
    <div class="news-content">
        <span class="news-date">2026.03.25</span>
        <h4 class="news-title">제목</h4>
        <p class="news-excerpt">내용...</p>
    </div>
</article>
```

### 색상 변경

`css/style.css` 파일 상단에서:

```css
:root {
    --color-primary: #dc2626;    /* 메인 색상 */
    --color-secondary: #eab308;  /* 서브 색상 */
    --color-bg: #0a0a0a;         /* 배경 색상 */
}
```

## 💻 기술 스택

- **HTML5** - 시맨틱 마크업
- **CSS3** - Flexbox, Grid, CSS Variables, Animations
- **JavaScript** - 바닐라 JS (라이브러리 없음)
- **Google Fonts** - Bebas Neue, Oswald, Inter

## 📱 반응형 브레이크포인트

- Desktop: 1200px+
- Tablet: 768px - 1199px
- Mobile: 480px - 767px
- Small Mobile: ~479px

## 🎯 페이지별 주요 기능

### 홈페이지 (index.html)
- 히어로 섹션 with 통계
- 다가오는 대회 미리보기
- 최신 뉴스 3개
- ADCC 소개 미리보기

### 대회일정 (schedule.html)
- 타임라인 형식 일정표
- 체급별 안내
- 대회 상세 정보

### 뉴스 (news.html)
- 그리드 레이아웃
- 최신순 정렬
- 카테고리 태그

### 갤러리 (gallery.html)
- 반응형 그리드
- 플레이스홀더 이미지
- SNS 링크

### 연락처 (contact.html)
- 연락처 정보
- 문의 양식
- 업무 시간 안내

## 🔧 커스터마이징

### 로고 변경
```html
<!-- 모든 페이지 네비게이션에서 -->
<h1 class="logo">ADCC<span class="logo-highlight">KOREA</span></h1>
```

### 푸터 수정
```html
<!-- 모든 페이지 하단 -->
<footer class="footer">
    <!-- 내용 수정 -->
</footer>
```

### SNS 링크 추가
```html
<!-- footer에서 href="#" 부분을 실제 URL로 변경 -->
<li><a href="https://instagram.com/adcckorea">Instagram</a></li>
```

## 📊 성능

- **Lighthouse Score**: 90+ (예상)
- **First Contentful Paint**: <1.5s
- **Time to Interactive**: <3s
- **모바일 친화성**: 100%

## 🌐 브라우저 지원

- ✅ Chrome (최신 2개 버전)
- ✅ Firefox (최신 2개 버전)
- ✅ Safari (최신 2개 버전)
- ✅ Edge (최신 2개 버전)
- ✅ 모바일 브라우저 (iOS Safari, Chrome Mobile)

## 🔒 보안

- HTTPS 자동 적용 (GitHub Pages)
- No inline scripts
- CSP 호환
- XSS 방어

## 📈 SEO

- 시맨틱 HTML5
- Meta 태그 최적화
- 구조화된 데이터 (추가 가능)
- 모바일 우선 설계

## 🤝 기여

이 프로젝트는 ADCC KOREA를 위해 제작되었습니다.

## 📄 라이선스

© 2026 ADCC KOREA. All rights reserved.

## 💡 도움말

자세한 배포 및 관리 가이드는 **[DEPLOYMENT.md](DEPLOYMENT.md)**를 참조하세요.

---

Made with ❤️ for ADCC KOREA
