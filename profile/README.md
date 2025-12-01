# 🧑‍🧑‍🧒🙋📞 GAMO 
안녕하세요. 시니어 맞춤 가족 소통 서비스 가모입니다.
\
[2025 성신여자대학교 융합캡스톤디자인 프로젝트]

<img src="https://github.com/user-attachments/assets/a164e657-8ca5-4b80-bfe4-2494e8a5e32d" width="70%" />

### 🤦‍♀️ 팀원 소개
<div align="center">

| Team Leader | Team Member | Team Member |
|:-----------:|:-----------:|:-----------:|
| <img src="https://github.com/pjhyun0225.png" width="100" /> | <img src="https://github.com/yjhss.png" width="100" /> | <img src="https://github.com/JiwonLee42.png" width="100" /> |
| [박지현](https://github.com/pjhyun0225)<br />키워드 추천, 편지 교정, 서버 배포 | [홍유진](https://github.com/yjhss)<br />편지 퍼블리싱, STT·SSE, 편지 API | [이지원](https://github.com/JiwonLee42)<br />영상통화·기록 UI 및 API, 녹음·STT API |

| Team Member | Team Member |
|:-----------:|:-----------:|
| <img src="https://github.com/chaehyeon02.png" width="100" /> | <img src="https://github.com/1siis1.png" width="100" /> |
| [이채현](https://github.com/chaehyeon02)<br />앨범 퍼블리싱, 앨범 API | [김시영](https://github.com/1siis1)<br />회원·가족 UI, 소셜 로그인·JWT, FE 레이아웃 |

</div>

## 📚 목차

1. [프로젝트 소개](#프로젝트-소개)  
2. [기술 스택](#-팀원-소개)  
3. [서비스 아키텍처](#-서비스-아키텍처)  
4. [프로젝트 구조](#프로젝트-구조)
5. [Git 협업 규칙](#-gitflow-규칙)


## ✨ **프로젝트 소개**
<div align="center">
  
### **프로젝트 목표**
<img src="https://github.com/user-attachments/assets/8674020b-2af9-4583-ac7d-c8095cb99c54" width="70%" />

### **소셜 기능**

<img src="https://github.com/user-attachments/assets/9ae1d411-cf8e-4eb6-8d58-0206b2c30a1b" width="70%" />

<img src="https://github.com/user-attachments/assets/ec9bd565-5822-41de-90c4-0bfaee2c6d72" width="70%" />

---

### **홈 화면**
<img src="https://github.com/user-attachments/assets/7178f87a-a110-426e-a6aa-97555dae374b" width="70%" />

---

### **가족 기능**
<img src="https://github.com/user-attachments/assets/f844ec24-3d15-4ff4-8b30-31533fd7ac3b" width="70%" />

<img src="https://github.com/user-attachments/assets/69ee2e55-e848-43da-90c2-471a3258fd45" width="70%" />

---

### **편지 기능**
<img src="https://github.com/user-attachments/assets/e4dc0478-a8a8-4299-849d-c2acd0857370" width="70%" />

<img src="https://github.com/user-attachments/assets/02374b93-0b1f-4ab9-998c-440ddf89880a" width="70%" />

---

### **영상통화 기능**
<img src="https://github.com/user-attachments/assets/dda28f68-5c81-44dc-9dbe-5aae10e18b24" width="70%" />

<img src="https://github.com/user-attachments/assets/cee5b807-387c-4105-905e-3af433aec911" width="70%" />

---

### **앨범 기능**
<img src="https://github.com/user-attachments/assets/3d4f5f9c-3302-4ee3-a76c-2699cba39912" width="70%" />

<img src="https://github.com/user-attachments/assets/a592d3ad-45d0-4c00-a0bc-768cae73c2e8" width="70%" />

</div>

### 🎦 GAMO 데모 영상
https://www.youtube.com/watch?v=aL9ShCryn3M


## 🛠 기술 스택

### Front-end  
<img src="https://skillicons.dev/icons?i=javascript,html,css,tailwindcss&theme=light" height="50">  
<img src="https://skillicons.dev/icons?i=webrtc&theme=light" height="50">

### Infra & Back-end  
<img src="https://skillicons.dev/icons?i=spring,fastapi,mysql,nginx,jenkins,gcp&theme=light" height="50">  

| 구분 | 기술 |
|------|------|
| **Language** | Java,Python |
| **Framework** | Spring Boot, FastAPI |
| **Database** | MySQL, JPA|
| **Infra** | GCP, Nginx |
| **CI/CD** | Jenkins |
| **Auth** | JWT, Spring Security |
| **기타** | OAuth, WebSocket, SSE, WebRTC, Google Cloud Storage |
| **외부 API** | Google Speech To Text, Gemini API |
| **frontend** | TailWindCss, HTML, Javascript, Thymeleaf  |

## ⛏️ 서비스 아키텍쳐
<div align="center">
<img width="90%" src="https://github.com/user-attachments/assets/9a8ad650-43c2-4543-b232-ac1fb1d32179" />
</div>

## 📁 프로젝트 구조
### Spring 레포지토리 폴더 구조 
```
src
├── frontend/                  # 프론트엔드 코드 (JS, CSS, Node 모듈)
│   ├── main.css               # 전역 스타일
│   ├── node_modules/          # 설치된 라이브러리
│   └── 각종 패키지별 서브 모듈
│
├── java/                      # 백엔드 코드
│   └── gamo/web/
│       ├── WebApplication.java 
│       ├── auth/              # 인증 관련
│       ├── common/            # 공통 유틸, 설정
│       ├── family/            # 가족 관련 기능
│       ├── home/              # 홈 화면 관련
│       ├── letter/            # 편지 기능
│       ├── member/            # 회원 관리
│       ├── photo/             # 사진/앨범 관리
│       └── videocall/         # 영상 통화 기능
│
├── resources/                 
│   ├── application.yml         # Spring 설정
│   ├── application-secret.properties 
│   ├── google-service-account.json   
│   ├── static/                # 정적 리소스(js, css, svg)
│   └── templates/             # Thymeleaf 템플릿
│       ├── fragments/         # 공통 레이아웃/모달
│       ├── login.html
│       └── pages/             # 기능별 페이지
│
├── package.json              
├── package-lock.json          
├── postcss.config.js          
└── tailwind.config.js         # Tailwind CSS 설정
```
### FastAPI 레포지토리 폴더 구조

```
GAMO_AI_API/
├── app/                 # 애플리케이션 코드
│   ├── core/            # 환경설정
│   ├── database/        # DB 연결 및 모델
│   ├── routers/         # API 엔드포인트
│   ├── utils/           # 유틸리티 함수
│   └── main.py          # 서버 실행 파일
├── venv/                # 가상 환경
├── .env                 # 환경 변수
├── .gitignore
├── Jenkinsfile          # 배포 스크립트
└── README.md

```

## 📍 Git 협업 규칙

- `develop` 브랜치에 직접 **commit/push 금지**  
- 작업 전 반드시 **issue 작성 후 Pull Request 연동**  
- Pull Request는 **2명 이상 코드 리뷰 후 merge**  
- 기능 개발 시:
  - `develop` → `feature/기능` 브랜치 생성
  - 기능 개발 완료 → PR 생성 → 리뷰 후 `develop` merge
