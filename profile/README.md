<div align="center">
  
<img width="3135" height="1126" alt="PNG 배사" src="https://github.com/user-attachments/assets/ab896379-e438-4dec-a6b9-0be9226a6934" />

  <br/>
  <br/>

  # Pick-N-Go (PNG)
  > **날씨, 골든아워, 이동 시간까지 한 번에 다 계산해 주는 스마트 여행 플래너** <br/>
  > 외부 API를 융합하여 이동 경로 최적화부터 날씨 기반 사진 촬영 타이밍까지 원스톱으로 제공합니다.

  <br/>

  ![Spring Boot](https://img.shields.io/badge/spring%20boot-%236DB33F.svg?style=for-the-badge&logo=spring-boot&logoColor=white)
  ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
  ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
  ![React Native](https://img.shields.io/badge/react_native-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
  ![Expo](https://img.shields.io/badge/expo-1C1E24?style=for-the-badge&logo=expo&logoColor=#000020)
  ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
  
  ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
  ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
  ![GitHub Actions](https://img.shields.io/badge/github%20actions-%232088FF.svg?style=for-the-badge&logo=github-actions&logoColor=white)
  ![Dependabot](https://img.shields.io/badge/dependabot-%234F5D95.svg?style=for-the-badge&logo=dependabot&logoColor=white)
  ![Google Gemini](https://img.shields.io/badge/google%20gemini-8E75B2?style=for-the-badge&logo=google%20gemini&logoColor=white)
  ![CodeRabbit](https://img.shields.io/badge/CodeRabbit-%23FF570A.svg?style=for-the-badge&logo=coderabbit&logoColor=white)

</div>

<br/>

## ✨ Core Features

- **스마트 코스 플래닝** : 가고 싶은 장소(스팟)를 담아 나만의 여행 코스를 자유롭게 생성 및 편집할 수 있습니다.
- **실시간 길찾기 자동화** : 코스 내 명소를 추가하거나 순서를 바꿀 때마다 **카카오모빌리티 API**가 실시간 교통정보를 반영해 총 이동 시간과 거리를 자동 계산합니다.
- **인생샷 골든아워 타이머** : 글로벌 일출/일몰 API를 활용하여 특정 장소에서 사진 찍기 가장 완벽한 시간(Golden Hour)을 추천해 줍니다.
- **스마트 날씨 & 알림 (예정)** : 기상청 단기예보를 기반으로, 내가 위시리스트에 담은 장소의 날씨가 맑아질 때 푸시 알림을 보내줍니다.

<br/>

## 🛠️ Tech Stack

### Backend
- **Framework:** Spring Boot 4.0.6, Spring Data JPA
- **Language:** Java 21
- **Database:** MySQL 8.0, Redis (예정)
- **API Client:** Spring WebFlux (WebClient)
- **Documentation:** Swagger (Springdoc OpenAPI)

### Frontend
- **Framework:** React Native 0.79, Expo 53
- **Language:** TypeScript 5.x
- **Styling:** NativeWind 4.x (Tailwind CSS v3)
- **Server State:** TanStack Query 5.x
- **Client State:** Zustand 5.x

### Infrastructure & DevOps
- **Cloud:** AWS (EC2, RDS, S3) / Docker

<br/>

## ⚙️ CI/CD & Workflow

프로젝트의 안정적인 운영과 효율적인 협업을 위해 자동화 인프라를 적극적으로 활용합니다.

- **GitHub Actions** : Git Tag 기반의 STG/PRD 서버 빌드 및 배포 자동화, 빌드 안정성 검증
- **Dependabot** : 주기적인 의존성 검사 및 보안 취약점 자동 감지, 패치 Pull Request 자동화
- **Google Gemini / CodeRabbit** : PR 생성 시 AI 코드 리뷰 자동화

<br/>

## 🔗 External APIs

Pick-N-Go는 사용자에게 최적의 경험을 제공하기 위해 아래의 외부 데이터들을 실시간으로 연동합니다.
- [Kakao Mobility API](https://developers.kakao.com/) - 차량 이동 시간 및 거리 계산
- [기상청 단기예보 조회서비스](https://www.data.go.kr/) - 스팟별 상세 기상 정보
- [Sunrise-Sunset API](https://sunrise-sunset.org/api) - 글로벌 일출/일몰 및 골든아워 데이터

<br/>

## 👋 Team Members

| 포지션 | 이름 | GitHub | 역할 및 담당 업무 |
|:---:|:---:|:---:|---|
| **FullStack** | 박예은 | [@yeni023](https://github.com/yeni023) | 온보딩 및 홈 화면, 3단계 확장형 지도 뷰, 스팟 상세(정보) 및 커뮤니티 피드 기능 구현 |
| **FullStack** | 모정민 | [@mozmin](https://github.com/mozmin) | 여행 계획(코스) 플래닝, 외부 API(길찾기/날씨/골든아워) 연동, 위시리스트 알림 시스템 구축 |
| **FullStack** | 소영재 | [@YoungjaeSo](https://github.com/YoungjaeSo) | 이메일/소셜 로그인 인증, 스팟 실시간 채팅, 사진 등록(EXIF 파싱) 및 풀스크린 뷰어 구현 |
| **FullStack** | 이예인 | [@yeainlee](https://github.com/yeainlee) | 통합 검색 기능, 주간 콘테스트 시스템, 커뮤니티 게시물 작성, 마이페이지/프로필 구현 |

<br/>

## 📁 Repository Structure

우리 팀은 프론트엔드와 백엔드를 각각 독립된 레포지토리로 관리합니다.
- [**PNG_backend**](https://github.com/Pick-N-Go/PNG_backend) : Spring Boot 기반의 백엔드 API 서버
- [**PNG_frontend**](https://github.com/Pick-N-Go/PNG_frontend) : React Native 기반의 프론트엔드 앱
