<div align= "center">
    <img src="https://capsule-render.vercel.app/api?type=soft&color=0:,100:030303&height=120&text=HUEFLIX&animation=&fontColor=ffffff&fontSize=70" />
</div>

![image](https://github.com/SuinShin/Hueflix/assets/148019115/a440f894-eb3c-43ca-91db-a089a358c420)

<div style="text-align: left;">
    <h2 style="border-bottom: 1px solid #d8dee4; color: #282d33;"> 🛠️ Tech Stacks </h2>
    <div style="margin: ; text-align: left;" "text-align: left;"> <img src="https://img.shields.io/badge/Apache Tomcat-F8DC75?style=flat-square&logo=Apache Tomcat&logoColor=white">
          <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=CSS3&logoColor=white">
          <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=HTML5&logoColor=white">
          <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=Java&logoColor=white">
          <img src="https://img.shields.io/badge/Javascript-F7DF1E?style=flat-square&logo=Javascript&logoColor=white">
          <img src="https://img.shields.io/badge/Oracle-F80000?style=flat-square&logo=Oracle&logoColor=white">
          <img src="https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=Spring&logoColor=white">
    </div>
</div>
    
## 📃Contents

1. [프로젝트 개요](#프로젝트-개요)<br>
2. [프로젝트 내용](#프로젝트-내용)<br>
3. [화면 별 기능 설명](#화면-별-기능-설명)<br>
4. [소감](#소감)<br>
   

## 📌팀 프로젝트 개요
- 프로젝트명: HueFlix

- 개발 인원: 7명

- 일정: 2023년 12월 4일 ~ 2023년 12월 22일
  
- 개발 목적: 박스오피스 영화의 정보를 공유하고 회원들의 평점 정보 확인,<br>
            댓글로 의견을 공유하는 웹 사이트 제작. 
  
- 개발 환경
    - Server: Apache-tomcat-9.0.0
    - Java EE: Eclipse (version 2023-06)
    - Database: Oracle SQL developer
    - Language: Java, Jsp, HTML, CSS, JavaScript, SQL, Spring Legacy, mybatis
    - Framework: Spring Tool suite 3.9.1
    - API: TMDB, KMDB

- 👩‍🔧 본인이 구현한 부분
  - 사이트 메인 화면, 로그인, 회원가입 창 UI (반응형 사이트 구현 - 창 크기, 디바이스 별로 UI 조정)
  - Spring Security를 이용한 회원 가입, 로그인
  - 권한 별 회원 메뉴 (헤더에서 로그인 한 회원의 드롭다운 메뉴)
  - 회원 정보 수정 페이지

## 🔎프로젝트 내용

- 팀원 역할

    - 공통: 웹사이트 UI 기획 및 구현, ERD 설계
    - 신민하: 영화정보 구현(영화 API 활용), 게시판 UI/UX 구현
    - 신수인: 메인 홈페이지 UI 및 로그인/회원가입 구현, 회원정보 수정 구현, 권한별 기능 구현
    - 임지선: 상영예정작 API를 활용하여 정보 구현, 메인 UI/UX 기능 구현, 영화상세정보 메뉴 기능 구현
    - 이도민: 공지사항 게시판 CRUD 구현, 댓글 구현, 영화정보 UI 구현
    - 심기훈: 영화정보의 평점 및 댓글 구현, 영화정보 UI/UX 구현, 공지사항 CRUD 구현
    - 김보성: 영화정보 UI 및 개발, 유지보수, 영화정보 UI/UX 구현
    - 박다진솔: 검색페이지 구현, 검색결과에서 영화 상세정보 이동 구현

- DB ERD 설계

![image](https://github.com/SuinShin/Hueflix/assets/148019115/48569f67-e6cf-421c-8328-8a4e334d8bb6)


## 🖥화면 별 기능 설명

## 메인

<details>
<summary>접기/펼치기</summary>

<br>

- 프로젝트를 실행하면 가장 먼저 표시되는 화면인 만큼, 시각적인 요소에 중점을 두었다.
- Swiper.js를 이용하여, 각 섹션별 영화의 정보와 랭킹을 TMDB에서 받아와 동적으로 슬라이드에 삽입하였다.
- JavaScript Ajax함수를 사용하여 TMDB API의 데이터를 요청하였다.
- API에서 반환한 JSON형식의 데이터를 받아와 처리하였다.
- 포스터를 클릭하면 해당 영화의 상세 정보 창으로 이동한다.

<br>

![image](https://github.com/SuinShin/Hueflix/assets/148019115/a58e2512-e1c4-481a-ba3d-e975635931ac)

<br>

- 해상도 별로 슬라이드의 갯수와 폰트 사이즈를 조정하여 반응형 웹을 구현했다.
- 화면 해상도에 따라 최소 2개 ~ 최대 7개 사이로 슬라이드 갯수가 동적으로 조정된다.

<br>

<img src="https://github.com/SuinShin/Hueflix/assets/148019115/57351974-80f8-4c35-9265-68d968cfacaa" width="300" height="1000">
<img src="https://github.com/SuinShin/Hueflix/assets/148019115/d2cf7595-ccd3-48aa-bd29-5ec1d4503a2d" width="700" height="1000">

<br><br>

- 영화 포스터에 마우스 오버를 하면 영화의 간단한 정보가 표시된다.

<br>

![image](https://github.com/SuinShin/Hueflix/assets/148019115/c4361298-9375-4372-84fb-c8b5f9aa9d10)


</details>


## 회원가입, 로그인

<details>
<summary>접기/펼치기</summary>

<br>

![image](https://github.com/SuinShin/Hueflix/assets/148019115/41af8506-aa43-4aaa-b144-c0ef7c39c743)
![image](https://github.com/SuinShin/Hueflix/assets/148019115/fcb7ab15-1779-469a-b224-c9a63b1807a1)

</details>



## 회원 정보 수정

## 현재 상영 중, 개봉 예정 메뉴

## 영화 상세 정보

## 공지사항 게시판

## 키워드 검색(영화, 영화인)

## 📓소감
