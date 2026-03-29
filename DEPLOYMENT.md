# ADCC KOREA 웹사이트 배포 가이드

이 가이드는 ADCC KOREA 웹사이트를 **완전 무료**로 GitHub Pages에 배포하는 방법을 설명합니다.

## 🚀 빠른 시작 (10분 완성)

### 1단계: GitHub 계정 만들기

1. [GitHub.com](https://github.com) 방문
2. 우측 상단 **Sign up** 클릭
3. 이메일, 비밀번호, 사용자명 입력
4. 이메일 인증 완료

### 2단계: 저장소(Repository) 만들기

1. GitHub 로그인 후 우측 상단 **+** 버튼 클릭
2. **New repository** 선택
3. 저장소 정보 입력:
   - Repository name: `adcc-korea` (또는 원하는 이름)
   - Public 선택 (무료)
   - ✅ **Initialize this repository with a README** 체크
4. **Create repository** 클릭

### 3단계: 파일 업로드

#### 방법 A: 웹 인터페이스에서 업로드 (가장 쉬움)

1. 생성된 저장소 페이지에서 **Add file** → **Upload files** 클릭
2. 모든 웹사이트 파일을 드래그 앤 드롭:
   ```
   index.html
   schedule.html
   news.html
   about.html
   gallery.html
   contact.html
   css/style.css
   js/main.js
   ```
3. 하단 **Commit changes** 클릭

#### 방법 B: GitHub Desktop 사용 (추천)

1. [GitHub Desktop](https://desktop.github.com/) 다운로드 및 설치
2. GitHub Desktop에서 로그인
3. **File** → **Clone repository** → 생성한 저장소 선택
4. 로컬 폴더에 웹사이트 파일 복사
5. GitHub Desktop에서 변경사항 확인
6. 좌측 하단에 커밋 메시지 입력 (예: "Initial website upload")
7. **Commit to main** 클릭
8. 상단 **Push origin** 클릭

### 4단계: GitHub Pages 활성화

1. 저장소 페이지에서 **Settings** 탭 클릭
2. 좌측 메뉴에서 **Pages** 선택
3. **Source** 섹션에서:
   - Branch: **main** 선택
   - Folder: **/ (root)** 선택
4. **Save** 클릭
5. 1-2분 후 페이지 상단에 URL 표시:
   ```
   https://[사용자명].github.io/adcc-korea/
   ```

## 🌐 커스텀 도메인 연결 (선택사항)

### 도메인 구매 (연 15,000원)

**추천 업체:**
- Cafe24 (한국어, 쉬움): https://www.cafe24.com
- GoDaddy (글로벌): https://www.godaddy.com
- Namecheap (저렴): https://www.namecheap.com

**추천 도메인:**
- `adcckorea.com` (1년: 약 15,000원)
- `adcckorea.co.kr` (1년: 약 18,000원)

### 도메인 연결 방법

1. **도메인 업체에서 DNS 설정:**
   - A 레코드 추가:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - CNAME 레코드 추가:
     ```
     www → [사용자명].github.io
     ```

2. **GitHub Pages에서 설정:**
   - Settings → Pages → Custom domain
   - 구매한 도메인 입력 (예: `adcckorea.com`)
   - ✅ **Enforce HTTPS** 체크 (SSL 자동 활성화)
   - **Save** 클릭

3. **적용 대기:**
   - DNS 전파: 최대 48시간 (보통 1-2시간)
   - SSL 인증서 발급: 자동 (무료)

## 📝 콘텐츠 수정 방법

### 1. 텍스트 수정

**HTML 파일 직접 수정:**
```html
<!-- index.html에서 -->
<h2 class="hero-title">
    THE ULTIMATE<br>
    <span class="hero-title-highlight">GRAPPLING</span><br>
    SHOWDOWN
</h2>
```

이 부분을 원하는 텍스트로 변경하세요.

**대회 일정 수정:**
`schedule.html` 파일에서 날짜와 정보 변경:
```html
<div class="date-month">APR</div>
<div class="date-day">15</div>
<div class="date-year">2026</div>
```

### 2. 색상 변경

`css/style.css` 파일 상단의 CSS 변수 수정:
```css
:root {
    --color-primary: #dc2626;  /* 빨강 → 원하는 색으로 변경 */
    --color-secondary: #eab308; /* 노랑 → 원하는 색으로 변경 */
}
```

**색상 코드 참고:**
- 빨강: `#dc2626`
- 파랑: `#2563eb`
- 초록: `#16a34a`
- 보라: `#9333ea`
- 주황: `#ea580c`

### 3. 이미지 추가

1. `images` 폴더 생성 (없으면)
2. 이미지 파일 업로드
3. HTML에서 placeholder 부분 수정:
```html
<!-- 기존 -->
<div class="news-image-placeholder">
    <span>NEWS</span>
</div>

<!-- 이미지로 변경 -->
<img src="images/news-1.jpg" alt="뉴스 이미지" style="width: 100%; height: 200px; object-fit: cover;">
```

## 🔄 업데이트 방법

### GitHub Desktop 사용:
1. 로컬 파일 수정
2. GitHub Desktop에서 변경사항 확인
3. 커밋 메시지 입력
4. **Commit to main** → **Push origin** 클릭
5. 1-2분 후 사이트 자동 업데이트

### 웹 인터페이스 사용:
1. GitHub 저장소에서 수정할 파일 클릭
2. 우측 상단 연필 아이콘 (Edit) 클릭
3. 내용 수정
4. 하단 **Commit changes** 클릭
5. 1-2분 후 사이트 자동 업데이트

## 💰 비용 정리

| 항목 | 비용 | 비고 |
|------|------|------|
| **GitHub Pages 호스팅** | **무료** | 무제한 트래픽 |
| **SSL 인증서 (HTTPS)** | **무료** | 자동 발급 |
| **도메인 (선택)** | 연 15,000원~ | 없어도 무방 |
| **총 비용** | **0원 ~ 15,000원/년** | |

## ⚡ 성능 최적화 (선택사항)

### 이미지 최적화
- [TinyPNG](https://tinypng.com/) 사용하여 이미지 압축
- 권장 크기: 1200px 이하

### 로딩 속도 개선
- CSS/JS 파일은 그대로 사용 (이미 최적화됨)
- 이미지 WebP 포맷 사용 권장

## 🆘 문제 해결

### 사이트가 보이지 않을 때:
1. Settings → Pages에서 URL 확인
2. 1-2분 대기 (첫 배포는 시간 소요)
3. 브라우저 캐시 삭제 (Ctrl+Shift+R)

### 도메인 연결이 안 될 때:
1. DNS 전파 대기 (최대 48시간)
2. [DNS Checker](https://dnschecker.org)에서 확인
3. HTTPS 체크박스 해제 후 재시도

### 수정사항이 반영되지 않을 때:
1. GitHub에서 파일 업데이트 확인
2. Actions 탭에서 배포 상태 확인
3. 브라우저 시크릿 모드로 접속

## 📱 모바일 최적화

이 웹사이트는 반응형으로 제작되어 모바일에서도 완벽하게 작동합니다.
- 자동으로 화면 크기에 맞춰 조정
- 모바일 메뉴 자동 지원
- 터치 인터랙션 최적화

## 🔐 보안

- GitHub Pages는 자동으로 HTTPS 적용
- DDoS 방어 기능 내장
- 백업은 GitHub에 자동 저장

## 📞 추가 도움이 필요하면

- GitHub Pages 공식 문서: https://docs.github.com/pages
- GitHub 커뮤니티: https://github.community

---

**축하합니다! 🎉**
이제 ADCC KOREA의 공식 웹사이트가 완전 무료로 운영됩니다!
