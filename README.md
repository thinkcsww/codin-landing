# CODIN 랜딩페이지

정적 단일 페이지 랜딩사이트입니다. 빌드 도구 없이 `index.html` 하나로 동작합니다.
Apple 개발자 심사용으로 "실제 운영 중인 서비스"임을 보여주는 회사 소개 랜딩입니다.

## 구성
- `index.html` — 랜딩페이지 본체 (Tailwind CDN + Pretendard + Iconify, 인라인 스타일/스크립트)
- `favicon.svg` — 파비콘
- `vercel.json` — 정적 배포 설정 (cleanUrls, 보안 헤더)

## 로컬 미리보기
```bash
npx serve .
# 또는
python3 -m http.server 8080
```
브라우저에서 `http://localhost:8080` 접속.

## Vercel 배포

### 방법 1 — CLI
```bash
npm i -g vercel
vercel        # 미리보기 배포
vercel --prod # 프로덕션 배포
```
프레임워크 프리셋은 **Other**, 빌드 명령 없음, 출력 디렉터리는 루트(`.`)로 두면 됩니다.

### 방법 2 — GitHub 연동
1. 이 폴더를 GitHub 저장소로 푸시
2. vercel.com → New Project → 저장소 선택
3. Framework Preset: **Other**, Build Command 비움 → Deploy

## Apple 심사 제출 시
App Store Connect의 마케팅 URL / 지원 URL 에 배포된 도메인을 입력하세요.
문의 이메일은 `hello@codin.app` 로 표기되어 있으니 실제 수신 가능한 주소로 교체하세요.
