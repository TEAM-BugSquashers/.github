# Scenestra 
![Image (12)](https://github.com/user-attachments/assets/6b293636-ec05-4a0a-b91d-99f546fec3d5)

## 목차
- [팀 소개](#팀-소개)
- [ERD](#erd)
- [개발환경](#개발환경)
- [화면 구성](#화면-구성)
- [요구사항](#요구사항)
- [주요 기능](#주요-기능)
- [주요 API](#주요-api)


## 팀 소개
#### 🐣 최준우
  - 팀장
    - Front / Back
      - 헤더/푸터/사이드바, 전체 목록 페이지, 검색 결과 페이지, 후기게시판 페이지, 관리자 페이지, 관리자 API

#### <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Animals/Seal.png" alt="Seal" width="25" height="25" /> 홍형석 
  - 팀원 
    - Back 
      - DB 테이블 생성, 사용자 인증 및 인가, 회원가입 기능, 이미지 업로드 처리, 예약 API, 상영관 API, 개인정보 수정 기능

#### 🐨 임현빈 
  - 팀원 
    - Back 
      - 영화 데이터 구축, 영화 API, 장르 API, 후기 API

#### 🐱 김유민 
  - 팀원 
    - Front 
      - 추천 페이지, 영화 상세 정보 팝업, 예약 페이지, 서비스 소개 페이지

#### 🐯 윤새르미 
  - 팀원 
    - Front / Back 
      - 로그인 페이지, 회원가입 페이지, 마이페이지, 관리자 API, ID/PW 찾기 기능

## ERD
![image (15)](https://github.com/user-attachments/assets/e6c1b050-abab-4220-941c-d43eebe9267c)


## 개발환경

### Tool
![IntelliJ](https://img.shields.io/badge/IntelliJ_IDEA-000000.svg?style=for-the-badge&logo=intellij-idea&logoColor=white)
![PyCharm](https://img.shields.io/badge/PyCharm-000000.svg?&style=for-the-badge&logo=PyCharm&logoColor=white)
![git](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)
![github](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)

### Infra
![aws](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)
<img src="https://img.shields.io/badge/Amazon%20EC2-FF9900?style=for-the-badge&logo=Amazon%20EC2&logoColor=white">
<img src="https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=Amazon%20S3&logoColor=white">
<img src="https://img.shields.io/badge/RDS-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white">

### DB
![Mysql](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
<img src="https://img.shields.io/badge/heidisql-47A248?style=for-the-badge&logo=heidisql&logoColor=white">
<img src="https://img.shields.io/badge/dbeaver-382923?style=for-the-badge&logo=dbeaver&logoColor=white">

### FrontEnd
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
<img src="https://img.shields.io/badge/vite-646CFF?style=for-the-badge&logo=vite&logoColor=white">
![NodeJS](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)
![HTML](https://img.shields.io/badge/HTML-239120?style=for-the-badge&logo=html5&logoColor=white)
![JS](https://img.shields.io/badge/p5%20js-ED225D?style=for-the-badge&logo=p5dotjs&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-239120?&style=for-the-badge&logo=css3&logoColor=white)
<img src="https://img.shields.io/badge/axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white">

### BackEnd
![SpringBoot](https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
<img src="https://img.shields.io/badge/JPA-6DB33F?style=for-the-badge&logo=java&logoColor=white">
![SpringSecurity](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=Spring-Security&logoColor=white)
![Jwt](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)
![Swagger](https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white)

## 화면 구성


## 요구사항

### 서버 요구사항
- JDK 17
- 


## 주요 기능


## 주요 api

### 인증 관련 API
- GET `/login` : 로그인 페이지
- POST `/login` : 로그인 처리
- GET `/logout` : 로그아웃

### User API
- GET `/api/users/me` : 내 정보 조회
- POST `/api/users/join` : 회원가입
- GET `/api/users/check-username` : 아이디 중복 체크
- GET `/api/users/preferred-genres` : 선호 장르 조회
- PUT `/api/users/preferred-genres` : 선호 장르 수정
- PUT `/api/users/info` : 유저 정보 수정
- PUT `/api/users/password` : 비밀번호 수정

### Theater API
- GET `/api/theaters` : 상영관 목록 전체 조회
- GET `/api/theaters/capacity` : 수용 가능 상영관 목록 조회
- GET `/api/theaters/{theaterId}` : 상영관 상세 조회

### Review API
- POST `/api/reviews(Content-Type: multipart/form-data)` : 게시글 작성
- GET `/api/reviews` : 전체 리뷰 목록 조회
- GET `/api/reviews/{id}` : 리뷰 상세 조회
- GET `/api/reviews/theater/{theaterId}` : 상영관 별 리뷰 목록 조회

### Reservation API
- GET `/api/reservations/available-dates` : 월별 상영관 예약 가능일 목록 조회
- GET `/api/reservations/available-times` : 특정 날짜에 예약 가능한 시간 목록 조회
- POST `/api/reservations/check-availability` : 상영관 예약 가능 여부 최종 조회
- POST `/api/reservations` : 상영관 예약
- GET `/api/reservations/{reservationId}` : 예약 상세 조회
- DELETE `/api/reservations/{reservationId}` : 예약 취소
- GET `/api/reservations/my/all` : 내 예약 목록 조회
- GET `/api/reservations/my/in-progress` : 내 진행 중인 예약 목록 조회

### Movie API
- GET `/api/movies` : 전체 영화 조회
- GET `/api/movies/{movieId}` : 영화 상세 조회
- GET `/api/movies/genres` : 전체 장르 조회
- GET `/api/movies/grouped-by-genre` : 장르별 영화 조회
- GET `/api/movies/genres/{genreId} : 해당 장르에 대한 전체 영화 조회
- GET `/api/movies/new` : 최신 영화 조회
- GET `/api/movies/best` : 인기(누적관객수) 영화 조회
- GET `/api/movies/recommend` : 추천 페이지
- GET `/api/movies/search` : 영화명으로 영화 검색

### Admin API
- GET `/api/admin/users` : 모든 사용자 조회
- GET `/api/admin/reservations` : 모든 예약 조회
- GET `/api/admin/reservations/{reservationId} : 예약 상세 조회




