# Next.js Enterprise Lab

본 저장소는 확장 가능하고 고성능의 **프런트엔드 아키텍처 설계의 모범 사례**를 보여주기 위한 연구소입니다.

## 🏗 아키텍처 및 패턴
- **Next.js 14 App Router**: 최신 React 서버 컴포넌트(RSC) 활용
- **Zustand**: 가볍고 직관적인 상태 관리
- **Atomic Design 기반 컴포넌트 구조**: 재사용성을 극대화한 설계
- **TypeScript**: 엄격한 타입 체크를 통한 안정성 확보

## 🛠 Tech Stack
- **Framework**: Next.js 14
- **State**: Zustand / TanStack Query
- **Styling**: Tailwind CSS / CSS Modules
- **DevOps**: Docker (Multi-stage), GitHub Actions

## 📖 Tech Wiki / Engineering Insights

### 1. Server Components vs Client Components
모든 컴포넌트는 기본적으로 Server Component로 작성하여 번들 사이즈를 줄이고 SEO를 최적화합니다. 상호작용이 필요한 부분만 Client Component로 분리하여 성능을 극대화했습니다.

### 2. 효율적인 상태 관리 전략
전역 상태는 최소화하고, URL 파라미터나 서버 사이드 상태를 적극 활용합니다. 복잡한 클라이언트 상태는 Zustand를 통해 중앙에서 관리합니다.

## 🚀 DevOps
- **Dockerfile**: `node:alpine` 기반의 멀티 스테이지 빌드 적용
- **CI**: GitHub Actions를 통한 빌드 및 린트 자동화
