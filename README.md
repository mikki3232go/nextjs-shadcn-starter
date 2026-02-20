# Next.js + shadcn/ui Starter Kit

Next.js 15, Tailwind CSS v4, shadcn/ui가 미리 설정된 스타터 킷입니다.

## 기술 스택

| 기술 | 버전 | 설명 |
|------|------|------|
| Next.js | 15 | App Router, Server Components |
| React | 19 | 최신 React |
| TypeScript | 5 | 타입 안전성 |
| Tailwind CSS | v4 | 유틸리티 CSS |
| shadcn/ui | 최신 | UI 컴포넌트 라이브러리 |
| next-themes | - | 다크모드 지원 |
| lucide-react | - | 아이콘 라이브러리 |

## 시작하기

```bash
# 의존성 설치
npm install

# 개발 서버 실행
npm run dev

# 프로덕션 빌드
npm run build
```

개발 서버: http://localhost:3000

## 프로젝트 구조

```
src/
├── app/
│   ├── layout.tsx          # 루트 레이아웃 (헤더, 푸터 포함)
│   ├── page.tsx            # 홈 페이지
│   ├── dashboard/
│   │   └── page.tsx        # 대시보드 예제 페이지
│   └── components/
│       └── page.tsx        # 컴포넌트 쇼케이스 페이지
├── components/
│   ├── layout/
│   │   ├── Header.tsx      # 헤더 (네비게이션, 다크모드 토글)
│   │   └── Footer.tsx      # 푸터
│   ├── providers/
│   │   └── ThemeProvider.tsx  # 다크모드 프로바이더
│   └── ui/                 # shadcn/ui 컴포넌트
└── lib/
    └── utils.ts            # 유틸리티 함수 (cn)
```

## 포함된 shadcn/ui 컴포넌트

- Button
- Card
- Input
- Label
- Badge
- Avatar
- DropdownMenu
- NavigationMenu
- Sheet
- Separator

## shadcn/ui 컴포넌트 추가

```bash
npx shadcn@latest add [컴포넌트명]

# 예시
npx shadcn@latest add dialog
npx shadcn@latest add table
npx shadcn@latest add form
```

## 기능

- 다크모드 지원 (시스템 설정 자동 감지)
- 반응형 레이아웃
- 모바일 사이드 메뉴 (Sheet 컴포넌트)
- TypeScript 완전 지원
- `any` 타입 없는 타입 안전 코드
