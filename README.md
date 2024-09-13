# :seedling: SeSAC 2차 프로젝트 Smile Hub
<br/>

## <img src="https://github.com/user-attachments/assets/d32dab93-440f-413f-b380-d70518a612ca" alt="Smile Hub" width="30"/> 프로젝트 소개개


* 주제 : **새상품** 정보를 알 수 있는 중고거래 사이트
* 기획 의도 : 중고상품 구매 시 새상품 가격 비교를 위한 다른 사이트 방문의 번거러움을 줄이고자 함.
* 기간 : 2024.08.26 ~ 2024.09.13
* Test ID: admin@admin.com
* Test Password: Admin12@1

<br>

## :raising_hand: Developers

| 팀원     | 역할          | 작업                                                         |
|:----------:|:---------------:|--------------------------------------------------------------|
| 석원준 [<img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white"/>](https://github.com/ymind14563)  | 백        | 유저 CRUD, 마이페이지, Money 충전, 프로필 업로드 (S3), 채팅 (socket), 리뷰 CRUD, 관리자 페이지 |
|          |  프론트    | 채팅, 관리자 페이지                    |
|          |  서버 배포     | AWS                                                         |
| 유예진 [<img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white"/>](https://github.com/yjyoo6831)   |  백        | 상품 CRUD, 새상품 데이터 가져오기 (네이버 API), 마이페이지: 찜 / 구매 / 판매 내역, 배송 현황   |
|          |  프론트    | 상품 CRUD UI                                                |
| 이유나 [<img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white"/>](https://github.com/youna99)  |  프론트   | Header, 로그인 / 회원가입 (카카오 주소 API), 마이페이지: 프로필, Money 충전, 찜 / 구매 / 판매 내역, 배송 현황, 상품 CRUD UI |

#### 석원준 [![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/ymind14563)
- **백엔드** : 유저 CRUD, 마이페이지, Money 충전, 프로필 업로드 (S3), 채팅 (socket), 리뷰 CRUD, 관리자 페이지
- **프론트엔드** : 채팅, 관리자 페이지
- **서버 배포**(AWS)

#### 유예진 [![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/yjyoo6831)
- **백엔드** : 상품 CRUD, 새상품 데이터 가져오기 (네이버 API), 마이페이지( 찜 / 구매 / 판매 내역, 배송 현황 )
- **프론트엔드** : 상품 CRUD

#### 이유나 [![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/youna99)
- **프론트엔드** : Header, 로그인 / 회원가입 (카카오 주소 API), 마이페이지( 프로필, Money 충전, 찜 / 구매 / 판매 내역, 배송 현황 ), 상품 CRUD UI


<br>

## :computer: Architecture

* Front-end: 
<img src="https://img.shields.io/badge/ejs-B4CA65?style=flat&logo=ejs&logoColor=white"/>  <img src="https://img.shields.io/badge/CSS-1572b6?style=flat&logo=css3&logoColor=white"/>  <img src="https://img.shields.io/badge/tailwind-06B6D4?style=flat&logo=tailwindcss&logoColor=white"/>   <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=333333"/> <img src="https://img.shields.io/badge/Axios-5a29e4?style=flat&logo=axios&logoColor=white"/> <img src="https://img.shields.io/badge/jQuery-0769AD?style=flat&logo=jquery&logoColor=white"/> <img src="https://img.shields.io/badge/Swiper-6332F6?style=flat&logo=swiper&logoColor=white"/>    

* Back-end:
<img src="https://img.shields.io/badge/Node.js-5fa04e?style=flat&logo=Node.js&logoColor=white"/>   <img src="https://img.shields.io/badge/Express.js-000000?style=flat&logo=Express&logoColor=white"/>   <img src="https://img.shields.io/badge/Sequlize-52b0e7?style=flat&logo=sequelize&logoColor=white"/>

* DB: <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=MySQL&logoColor=white"/>

* Tools: 
<img src="https://img.shields.io/badge/Visual Studio Code-007ACC?style=flat-square&logo=Visual Studio Code&logoColor=white"/>   <img src="https://img.shields.io/badge/MySQLWorkBench-4479A1?style=flat&logo=MySQL&logoColor=white"/>   <img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white"/>   <img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white"/>
* Deploy: <img src="https://img.shields.io/badge/Naver Cloud Platform-03c75a?style=flat&logo=naver&logoColor=white"/>   <img src="https://img.shields.io/badge/Apache-d22128?style=flat&logo=apache&logoColor=white"/>   <img src="https://img.shields.io/badge/Ubuntu-E95420?style=flat&logo=ubuntu&logoColor=white"/>
* Communication: 
<img src="https://img.shields.io/badge/Slack-4a154b?style=flat&logo=slack&logoColor=white"/>   <img src="https://img.shields.io/badge/Notion-000000?style=flat&logo=notion&logoColor=white"/>

<br>

## 📂 프로젝트 구조
- 프론트
```
├── /public
│   ├── images
│   ├── index.html
│   └── favicon.ico
├── /src
│   ├── /app : 애플리케이션의 전역 상태 관리, 라우팅
│   │   ├── ProtectedRouter.js
│   │   ├── rootReducer.js
│   │   ├── rootRouter.js
│   │   └── rootStore.js
│   ├── /features : Container Component (상태와 비즈니스 로직을 관리)
│   │   ├── Adimin
│   │   ├── Chat
│   │   ├── Product
│   │   └── User
│   ├── /pages : Presentational Component (UI, 화면 렌더링 역할)
│   │   ├── Adimin
│   │   ├── Chat
│   │   ├── Product
│   │   └── User
│   ├── /shared : 공통 Component 분리
│   │   ├── Header.js
│   │   ├── input.js
│   │   ├── Modal.js
│   │   └── ...
│   ├── App.js
│   ├── index.js
├── .eslintrc.js
├── .gitignore
├── .prettierrc
├── package-lock.json
├── package.json
├── README.md
├── postcss.config.js
└── tailwind.config.js
```
<br>

## :bulb: 요구사항 명세서
* API 명세서
<img src="./README_img/api명세서.png" style="width: 100%">
<br>
* 개발규칙 정의서
<img src="./README_img/개발규칙.png" style="width: 100%">

<br>

## :bulb: API 명세서

## 📚 데이터베이스 ERD

<img src="./README_img/ERD.JPG" style="width: 100%">

<br>


## :clipboard: 주요 페이지

### 로그인 / 회원가입
- 이메일, 닉네임 중복 검사 필수로 수행
<img src="https://github.com/user-attachments/assets/d156b0f9-4834-4a89-bf9a-25987a6e4d6d" style="width: 40%">
<img src="https://github.com/user-attachments/assets/ecf49708-907c-4190-a6eb-3aac30c53de7" style="width: 40%">

### 마이페이지
- 회원정보 수정, 탈퇴, 프로필 업로드 / 찜, 판매, 구매 내역 / 머니 충전
- 판매자, 구매자의 버튼 선택에 따른 배송 현황
<img src="https://github.com/user-attachments/assets/4193cb5e-1c3d-4758-b6e8-78b73249617f" style="width: 45%">
<img src="https://github.com/user-attachments/assets/dffbda73-ab22-4fc1-8829-658d749942b0" style="width: 45%">
<img src="https://github.com/user-attachments/assets/b246fd9c-1d18-4e43-9490-97b581597154" style="width: 50%">

### 채팅
- 구매자와 판매자의 양방향 소통 가능
<img src="https://github.com/user-attachments/assets/282b21cb-7244-4e43-a649-94326adc64fa" style="width: 70%">

### 메인, 검색
- 무한스크롤, 키워드로 검색
<img src="https://github.com/user-attachments/assets/abb54b8a-d0bc-4e3e-9304-21dd181c5692" style="width: 45%">
<img src="https://github.com/user-attachments/assets/3d6bb75e-3722-4e1f-8a25-f15217a620e5" style="width: 45%">

### 상세
- 상품 이미지 swiper, 배송 현황, 채팅/안전거래, 해당 상품의 최저가 목록(네이버 API)
<img src="https://github.com/user-attachments/assets/414f9b4e-c813-451a-8611-49698965606e" style="width: 45%">
<img src="https://github.com/user-attachments/assets/910de93f-b7a7-420a-b5c5-8b105349b291" style="width: 45%">

### 결제, 충전
- 금액 확인 후 결제 가능, money 충전을 통한 결제 구현
<img src="https://github.com/user-attachments/assets/73ba0d71-3d27-4357-a4b8-aae86d4fabdf" style="width: 40%">
<img src="https://github.com/user-attachments/assets/c2863f4f-8fe4-4038-a0ae-277b3d55c135" style="width: 40%">

### 상품 작성 및 수정, 삭제 
- 이미지 업로드 및 수정, 상품 삭제
<img src="https://github.com/user-attachments/assets/efe6a07b-a524-409d-8904-13fdf21ec20a" style="width: 50%">

### 관리자
- 회원 관리, 상품 관리 가능
<img src="https://github.com/user-attachments/assets/de6cd8cf-3ec0-43ae-8db5-220b117553e3" style="width: 50%">


