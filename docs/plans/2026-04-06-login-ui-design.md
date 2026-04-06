# Login UI Design

## Overview

이메일/비밀번호 기반 로그인/회원가입 UI. 백엔드 연결 없이 프론트엔드만 먼저 구현.

## Pages

- `/login` - 로그인/회원가입 탭 전환 폼

## Components

### LoginForm
- 이메일 입력 (이메일 형식 검증)
- 비밀번호 입력 (6자 이상)
- 로그인 버튼
- submit 시 alert로 확인 (백엔드 연결 전)

### SignupForm
- 이메일 입력 (이메일 형식 검증)
- 비밀번호 입력 (6자 이상)
- 비밀번호 확인 (일치 검증)
- 가입 버튼
- submit 시 alert로 확인 (백엔드 연결 전)

## File Structure

```
src/
  app/
    login/
      page.tsx          # 로그인 페이지 (Server Component wrapper)
  components/
    auth/
      LoginForm.tsx     # 로그인 폼 (Client Component)
      SignupForm.tsx    # 회원가입 폼 (Client Component)
```

## Styling

- Tailwind CSS
- 다크모드 지원 (dark: prefix)
- 중앙 정렬 카드 레이아웃

## Future

- 백엔드 연결 시 Server Action 또는 API Route로 전환
- 세션/토큰 관리 추가
