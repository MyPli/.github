# 🎧 MyPli

- 배포 URL:

- 테스트 메일: `test4@mail.com`

- 테스트 비밀번호: `test444`

<br />

## 프로젝트 소개
- **MyPli**는 사용자들이 좋아하는 영상을 모아 플레이리스트를 만들고, 이를 통해 취향을 공유하며 즐길 수 있는 새로운 웹 서비스입니다.
- 사용자는 YouTube API를 활용하여 자신만의 영상 컬렉션을 만들고 관리할 수 있습니다.
- 또한, 다른 사용자가 생성한 다양한 플레이리스트를 탐색하며 새로운 콘텐츠를 발견할 수 있습니다.
- 그리고, 마음에 드는 플레이리스트에 좋아요를 남기며 사용자 간의 상호작용을 즐길 수 있습니다.
- 간단하고 직관적인 인터페이스를 통해 나만의 음악, 영상 컬렉션을 생성하고, 다른 사람들의 플레이리스트를 탐색하며 소통할 수 있습니다.

## MyPli 팀
| [정동구](https://github.com/dongguJeong) | [심채윤](https://github.com/chaeyun-sim) | [조성민](https://github.com/Ss0Mae) | [김난영](https://github.com/Algoruu) |
| -- | -- | -- | -- |
| <img src="https://avatars.githubusercontent.com/u/133619736?v=4" width="120" /> | <img src="https://avatars.githubusercontent.com/u/111689342?v=4" width="120" /> | <img src="https://avatars.githubusercontent.com/u/80831228?v=4" width="120" />  | <img src="https://avatars.githubusercontent.com/u/126838925?v=4" width="120" />  |
| <p align="center">FE</p> | <p align="center">FE</p> | <p align="center">BE</p> | <p align="center">BE</p> |


## 프로젝트 실행하기
```
$ git clone https://github.com/MyPli/front.git
$ npm install
$ npm run dev
```

<br />

## 개발 환경
### 프론트엔드
![Next JS](https://img.shields.io/badge/Next-black?style=for-the-badge&logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![Zustand](https://img.shields.io/badge/zustand-%2320232a.svg?style=for-the-badge)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![React Query](https://img.shields.io/badge/-React%20Query-FF4154?style=for-the-badge&logo=react%20query&logoColor=white)
<br />
### 백엔드
![NestJS](https://img.shields.io/badge/nestjs-%23E0234E.svg?style=for-the-badge&logo=nestjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=Prisma&logoColor=white)
![Swagger](https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
<br />
### 협업 도구 및 배포
![Slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-%23000000.svg?style=for-the-badge&logo=notion&logoColor=white)
<img src="https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white" />
![Swagger](https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white)
![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)

<br />

## 폴더 구조
```
프론트엔드 개발 폴더 구조에 대한 설명을 작성해주세요
```

```
backend/
├── auth/                    # 인증 관련 로직 (JWT, Google OAuth)
│   ├── dto/                 # 인증 데이터 전송 객체
│   ├── guards/              # 인증 및 권한 관리
│   ├── strategies/          # 인증 전략
│   └── auth.*               # 인증 API, 서비스, 모듈
│
├── playlist/                # 플레이리스트 생성 및 관리
│   ├── dto/                 # 데이터 전송 객체
│   ├── entities/            # 플레이리스트 엔티티
│   └── playlist.*           # API, 서비스, 모듈
│
├── video/                   # 비디오 관리 기능
│   ├── dto/                 # 데이터 전송 객체
│   ├── entities/            # 비디오 엔티티
│   └── video.*              # API, 서비스, 모듈
│
├── user/                    # 사용자 정보 관리
│   ├── dto/                 # 사용자 데이터 전송 객체
│   ├── entities/            # 사용자 엔티티
│   └── user.*               # API, 서비스, 모듈
│
├── like/                    # 좋아요 기능
│   └── like.*               # API, 서비스, 모듈
│
├── search/                  # 검색 기능
│   └── search.*             # API, 서비스, 모듈
│
├── prisma/                  # 데이터베이스 설정 및 연동
│   └── prisma.*             # 서비스 및 모듈
│
├── s3/                      # AWS S3 연동
│   └── s3.*                 # 서비스 및 모듈
│
├── app.*                    # 메인 애플리케이션 설정 및 진입점
├── main.ts                  # 서버 엔트리포인트
└── schema.prisma            # Prisma 스키마 정의

```
- **[데이터베이스 설계 설명](https://clean-indigo-57d.notion.site/DB-MyPli-161382bd5b8e802f84cef03f22554247?pvs=4)**
<br />

## 트러블슈팅
- **[프론트엔드에서 하나 작성해주시면 될것 같습니다](https://)** 
- **[백엔드 트러블 슈팅 작성할 곳](https://)** 
  
<br />

## 주요 기능
| 회원가입/로그인 페이지 | 메인페이지 | 페이지 |
| -- | -- | -- |
|<img src="https://github.com/user-attachments/assets/" width="200" /> | <img src="https://github.com/user-attachments/assets/" width="200" /> | <img src="https://github.com/user-attachments/assets/" width="200" /> |

| 플레이리스트 생성 페이지 | 좋아요한 플레이리스트 페이지 | 마이페이지 |
| -- | -- | -- |
| <img src="https://github.com/user-attachments/assets/" width="200" /> |<img src="https://github.com/user-attachments/assets/" width="200" /> |<img src="https://github.com/user-attachments/assets/" width="200" />|

<br />

## 향후 개선 사항
 - 로딩 에러 처리의 개선 사항
 - 관리자 페이지 생성
 - 백엔드에서의 사진 관리
 - 리프레쉬 토큰과 로그아웃 구현
<br />
