# 📝 JPA 회원가입 & 로그인 프로젝트

Spring Boot와 JPA를 활용하여 **회원가입 및 로그인 기능**을 구현한 프로젝트입니다.  
간단한 CRUD, 세션 로그인/로그아웃 처리, 회원 목록 조회 및 삭제, 이메일 중복 체크 등을 연습하기 위해 제작했습니다.

---

## 🚀 기술 스택
- **Backend**: Spring Boot, Spring Web, Spring Data JPA
- **Database**: H2 (개발용), MySQL
- **View**: Thymeleaf, HTML
- **Frontend**: AJAX, JavaScript
- **Build Tool**: Gradle
- **Language**: Java 17

---

## 📂 프로젝트 구조
src/main/java/com/example/demo
├── controller # 웹 요청 처리
├── dto # DTO 클래스
├── entity # JPA 엔티티 클래스
├── repository # JPA Repository 인터페이스
├── service # 비즈니스 로직
└── DemoApplication.java

---

## ✨ 주요 기능
- 회원가입  
  - 이메일, 비밀번호, 이름 입력 후 DB 저장
- 로그인  
  - 이메일/비밀번호 일치 여부 확인
  - HttpSession을 활용하여 로그인 상태 유지
- 회원 목록 조회  
  - DB에 저장된 회원 리스트 출력
- 이메일 중복 체크 (AJAX 사용) 
  - 회원가입 시 입력한 이메일이 DB에 이미 존재하는지 비동기 요청으로 확인
- 회원 정보 수정, 회원 삭제
