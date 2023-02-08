# adultonly

  - 팀이 19팀이여서 19라는 이름에 맞도록 술집 관련 맛집을 추천하는 사이트로 성인들만 이라는 이름을 작성함

# 목차

1. **웹 서비스 소개**
2. **기술 스택**
3. **주요 기능**
4. **특이사항**
5. **개발 팀 소개**
6. **개발 기간 및 일정**
7. **프로젝트 후기**

<br>

# 1. 서비스 소개

<br>

## 입장시 로딩 페이지

![loading](https://user-images.githubusercontent.com/108659935/217586673-5d5e02bd-2e68-4f70-9a6e-01f5a94ae512.gif)

  - Canva에서 제작한 이미지로 처음 페이지 입장시 나오는 화면 구성
  - 자동 캐러셀로 이미지 반복하여 배경 보여줌

<br>

## 메인 페이지 및 검색 구현

![mainpage](https://user-images.githubusercontent.com/108659935/217594097-25b5d6a8-ecd0-4b8e-a681-8c2e880f50bc.gif)

  - 메인 페이지의 전체적인 화면 구성 및 좋아요 갯수로 인기 가게 캐러셀로 출력
  - 검색 자동완성 기능을 통해서 글자와 비슷한 가게 이름들 출력 및 이동

<br>

## 회원 가입

![signup](https://user-images.githubusercontent.com/108659935/217587538-ef4bfaa2-b2e2-4826-ba09-1d87a4f86e79.gif)

  - 회원 가입 페이지에서 아이디 유효성 검사 및 중복확인을 통해 중복된 아이디를 방지한다.
  - 비밀번호 유효성 검사를 통해서 비밀번호가 같은지 틀린지 체크해준다.
  - 이메일 입력란에서 직접 입력할 경우와 미리 설정된 도메인을 넣을경우 값이 자동변경 되도록 구현했다.
  - 직업 선택란에서 일반인인지 사장님인지를 통하여 가게 등록 및 리뷰작성이 가능하다.
  
<br>

## 로그인

![login](https://user-images.githubusercontent.com/108659935/217589139-52d912eb-3705-4050-a84b-70e88d3fc14f.gif)

  - 등록된 정보를 바탕으로 로그인을 통해 회원 정보 및 프로필 페이지로 자유롭게 이동이 가능하다.
  - 프로필 페이지에선 팔로우, 팔로워, 작성한 댓글, 작성한 게시글, 좋아요 누른 갯수 등이 표시된다.
  - 각 회원 별로 글을 무엇을 작성하였는지 보고 취향에 맞는 사람들끼리 팔로우를 할 수 있도록 회원목록 페이지에서 회원들이 서로 누가있는지 볼 수 있도록 구현하였다.

<br>

## 프로필 수정 및 프로필 바

![editinfo](https://user-images.githubusercontent.com/108659935/217590511-12df0261-4774-4e70-8f3e-c5b49b103705.gif)
  
  - 프로필 수정 페이지를 통하여 이름 변경, 이메일 주소 변경, 프로필 이미지 변경, 비밀번호 변경 등을 할 수 있다.
  
 ![editinfo2](https://user-images.githubusercontent.com/108659935/217591107-68a95987-8096-4d63-80cc-63d5a322bc57.gif)
  
  - 우측 위 프로필 모양을 누르면 어디서든 자유롭게 내 프로필 페이지로 이동이 가능하고 토글 버튼으로 선택할 수 있는 옵션을 넣었다.

<br>

## 맛집 리스트

![main](https://user-images.githubusercontent.com/108659935/217591594-36fbf6fd-1925-4bd1-8996-ab96bc68de71.gif)

  - 맛집 리스트의 테마별로 한식, 중식, 일식 등 필터링을 통해서 원하는 테마를 정하여 음식을 몰아서 볼 수 있다.

<br>

## 맛집 등록 및 가게 정보

![storeinfo](https://user-images.githubusercontent.com/108659935/217593248-b9c4dc9f-93f8-4c1f-b1dd-235cb95850e7.gif)

  - 회원가입 페이지에서 사장님으로 등록된 경우 맛집 등록버튼이 활성화 되며 카카오 API 지도를 가져와 주소를 찾을 수 있도록 구현했다.
  - 가게 정보들을 살펴보면 가게의 위치도 카카오 API를 통해서 위치를 표시해주고 있다.
  - 우측 상단의 마커표시를 누르면 좋아요로 가게가 등록되고 리뷰 작성을 통해서 리뷰를 달 수 있다.
  - 리뷰의 별점은 마우스 호버&드래그 효과로 별이 채워지도록 구현했다.
  - 비동기 댓글은 하지못했지만 동기로 댓글작성이 가능하다.

<br>

## 페이지 네이션 및 게시판 글 작성

![articles](https://user-images.githubusercontent.com/108659935/217595046-6999d8a0-a31f-4b2a-8033-06fea592b91f.gif)

  - 부트스트랩 페이지네이션을 가져와서 커스텀을 통해서 최대 5개를 출력하며 맨 마지막 페이지 이동 및 처음 페이지 이동을 구현함.
  - 유저간 소통가능한 자유게시판을 만들었고 글작성을 통해서 유저들간 소통이 가능하도록 구현함.
  - 유저가 이미지를 따로 넣지않을 경우 지정된 이미지를 출력해줌.


# 2. 기술 스택

| Frontend | Backend | Cooperation | Release |
| --- | --- | --- | --- |
| HTML5 | Python | Git | heroku |
| CSS3 | Django | GitHub |  |
| Bootstrap | SQLite | Notion |  |
| JavaScript |  | Discord |  |

<br>

# 3. 주요 기능

- `회원 가입 및 유효성 검사`
- `로그인`
- `CRUD`
- `검색기능`
- `유저간 팔로우 및 소통`
- `테마별 필터를 통한 맛집 검색`

<br>

# 4. 참고 자료


**페이지 구성 Figma**

![image](https://user-images.githubusercontent.com/108659935/217597659-ea3d080c-d726-4047-a0a7-db25bbdd40b1.png)

![image](https://user-images.githubusercontent.com/108659935/217597633-dd91fff5-de38-4f83-a801-8663a3816fd3.png)

![image](https://user-images.githubusercontent.com/108659935/217597709-67ae520e-7eaa-4c31-8635-7013af8298ed.png)

![image](https://user-images.githubusercontent.com/108659935/217597763-110b43f0-4592-4c24-883a-0064583344dd.png)

![image](https://user-images.githubusercontent.com/108659935/217597811-810b8857-ee47-45f0-8a77-0d14d5daeec8.png)

**모델 ERD 구성**

![image](https://user-images.githubusercontent.com/108659935/217596883-5dcb0466-66d6-4387-af4f-f8ba48312b9c.png)

**기획서**

<a href="https://www.notion.so/hg-edu/8fed2c0a53b94d1a9fbf303a7f2f5196">기획 Notion</a>

**노션 칸반보드 이용**

![image](https://user-images.githubusercontent.com/108659935/217596073-b336326c-f450-41de-8b6d-de384f7c07d1.png)

# 5. 개발 중 이슈

![image](https://user-images.githubusercontent.com/108659935/217596245-96092ae5-46ce-4455-8813-f0fd5c00f6dc.png)
![image](https://user-images.githubusercontent.com/108659935/217596316-c16cd03f-d6f6-470b-8db5-d7d5d3550fef.png)

  - 개발중 발생했던 이슈들에 대해서 해결하는데 시간이 걸렸던 문제들을 참고자료와 함께 정리함.


# 6. 개발 기간 및 일정

**개발 기간 : 10.31 (월) ~ 11.07 (월)

# 7. 내가 한 작업들

![image](https://user-images.githubusercontent.com/108659935/217598323-0823012c-ba4f-4b18-851e-6a2c8b850610.png)

![loading](https://user-images.githubusercontent.com/108659935/217586673-5d5e02bd-2e68-4f70-9a6e-01f5a94ae512.gif)

  - 화면 초기 페이지 구현 및 캐러셀 자동 슬라이드 구현

![image](https://user-images.githubusercontent.com/108659935/217598487-bf433a9f-b938-44be-9f9f-b505daadfad3.png)

  - 페이지에 사용될 색상 조합

![main](https://user-images.githubusercontent.com/108659935/217591594-36fbf6fd-1925-4bd1-8996-ab96bc68de71.gif)

  - 테마별 필터링 기능 구현

 ![signup](https://user-images.githubusercontent.com/108659935/217587538-ef4bfaa2-b2e2-4826-ba09-1d87a4f86e79.gif)
 
  - JS를 이용한 회원가입 유효성 검사 및 페이지 커스텀


# 8. 프로젝트 후기

  - 교육과정에서 마지막 프로젝트 주간에 들어서 처음으로 시작한 팀 프로젝트로 정해진 주제로 기획부터 설계까지 모두 우리가 직접 해야하는 작업인 만큼 처음 시작하기가 어려웠다.

  - 모두 같은 교육기간동안 같은 것을 배웠기 때문에 팀이름 짓는 것부터 어려웠고 팀의 이름에 맞는 주제를 잡기또한 어려웠다.

  - 울타리 안에서 생활하다 처음으로 밖으로 나온 기분이였다. 과정을 진행하는 동안은 가이드 안에서 주어진 틀대로 행동하다 백지상태에서 처음부터 기획하고 만들어 나가는 것이 무척 힘이들었고, ERD, Figma 등 툴에 익숙치 않아서 추상적으로만 만들었던 것 같다.

  - Bootstrap의 코드를 긁어오는 것이 아닌 직접 CSS를 조작하여 홈페이지를 자유롭게 꾸며보고 싶다는 생각이 들었다.

  - 로그인 및 회원가입의 경우 Django 내부에 포함된 모델이 아닌 직접 커스텀을 해보며 form 데이터가 어떤 식으로 전달되는지 이해할 수 있었고 JavaScript로 유효성 검사를 하는 방법을 익힐 수 있어서 값진 경험을 했다.

  - 유효성 검사를 진행하는 과정에서 부족한 JavaScript 지식으로 인해서 코드를 복사 붙여넣기 한 후 블로그 코드를 분석하여 커스텀을 하는데 시간을 많이 소비한 것이 아쉬움이 남는 프로젝트 였다.
