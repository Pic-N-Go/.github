<div align="center">
  
<img width="3135" height="1126" alt="PNG 배사" src="https://github.com/user-attachments/assets/ab896379-e438-4dec-a6b9-0be9226a6934" />


  <br/>
  <br/>

  # Pick-N-Go (PNG)
  > **날씨, 골든아워, 이동 시간까지 한 번에 다 계산해 주는 스마트 여행 플래너** <br/>
  > 외부 API를 융합하여 이동 경로 최적화부터 날씨 기반 사진 촬영 타이밍까지 원스톱으로 제공합니다.

  <br/>

  ![Spring Boot](https://img.shields.io/badge/Spring_Boot-4.0.6-6DB33F?style=flat-square&logo=springboot&logoColor=white)
  ![Java](https://img.shields.io/badge/Java-17-007396?style=flat-square&logo=java&logoColor=white)
  ![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=flat-square&logo=mysql&logoColor=white)

</div>

<br/>

## Core Features (핵심 기능)

- **스마트 코스 플래닝** : 가고 싶은 장소(스팟)를 담아 나만의 여행 코스를 자유롭게 생성 및 편집할 수 있습니다.
- **실시간 길찾기 자동화** : 코스 내 명소를 추가하거나 순서를 바꿀 때마다 **카카오모빌리티 API**가 실시간 교통정보를 반영해 총 이동 시간과 거리를 자동 계산합니다.
- **인생샷 골든아워 타이머** : 글로벌 일출/일몰 API를 활용하여 특정 장소에서 사진 찍기 가장 완벽한 시간(Golden Hour)을 추천해 줍니다.
- **스마트 날씨 & 알림 (예정)** : 기상청 단기예보를 기반으로, 내가 위시리스트에 담은 장소의 날씨가 맑아질 때 푸시 알림을 보내줍니다.

<br/>

## Tech Stack (기술 스택)

### Backend
- **Framework:** Spring Boot 3.x, Spring Data JPA
- **Language:** Java 17
- **Database:** MySQL 8.0, Redis (예정)
- **API Client:** Spring WebFlux (WebClient)
- **Documentation:** Swagger (Springdoc OpenAPI)

### Frontend
- **Framework:** React Native
- **Styling:** 

### Infrastructure & DevOps
- **Cloud:** AWS (EC2, RDS, S3) / Docker
- **CI/CD:** GitHub Actions

<br/>

## 🔗 External APIs

Pick-N-Go는 사용자에게 최적의 경험을 제공하기 위해 아래의 외부 데이터들을 실시간으로 연동합니다.
- [Kakao Mobility API](https://developers.kakao.com/) - 차량 이동 시간 및 거리 계산
- [기상청 단기예보 조회서비스](https://www.data.go.kr/) - 스팟별 상세 기상 정보
- [Sunrise-Sunset API](https://sunrise-sunset.org/api) - 글로벌 일출/일몰 및 골든아워 데이터

<br/>

## Team Members (팀원 소개)

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
- [**PNG_frontend**](https://github.com/Pick-N-Go/PNG_frontend) : React 기반의 프론트엔드 웹/앱 화면
