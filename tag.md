깃헙에서도 코딩할 수 있음(바로 커밋 생성) - 간단한 수정 추천(많이 수정해야하면 로컬에서 하는게 유리)

깃헙에서 리드미 작성 --> 새로운 커밋생성하므로 Commit changes 누른다

ai가 제목 지어주는데 새로고침 해서 바꿀 수 있음

원격 = remote
앞에 있는 작업물(원격, 동료도 업로드 가능)을 main(로컬)으로 가져오려면 Pull()fetch+merge) 써야함
--> 원격( origin main)은 같은 브랜치지만 이름만 같이 다름. 
-> 일단 통쨰로 가져와서 내 저장소에 main과 origin main이 같이 공존(fetch) --> 다른 분기가 생기거나 동료가 만든 것 때문에 conflict 가능
pull = fetch와 merge가 반복적으로 발생하는 것

vs code 켜는 법 터미널에서 code .

메인이 뒤에있었으므로 앞으로 가야해 FF 됨
--> fetch와 merge가 같이 일어난다는 뜻

팀장이 레포 만들어 놓고 협업자(콜라보레이터)로 팀원들을 등록해놓으면 로컬에서 만든 걸 원격에 올림 -> 팀원들에게 제가 만들었으니 풀 하시면 됩니다. --> 실시간 반복 --> 같은 상태 코드 공유하면서 작업계속. 누군가 만들었으면 ㅂ마로 풀 할 필요는 없고 다하고 하면된다. conflict 날 수 있는 부분은 서로 협의를 통해 잘 알아두고 서로 중복 작업을 하지 않도록 잘 협의 (계속 아침에 회의를 통해 협의 해야함) --> 실제로는 안 내기 힘들다(ai때문에 더 빨라짐. 정확하게 어디를 하라고 짚어주지 않으면 광범위하게 작성해버림

--> 바이브 코딩 시 작업할 곳을 조금씩 조금씩 하는게 좋다, 합치기 어려우므로

###ISSUES###
팀작업시 이슈레이징 팀끼리 해도 좋다(잊어버릴 수 있으므로 반드시 이슈에 기록) Issue log
--> 예, 리드미가 부실하다고 생각될시 --> Update readme, 내용에 작업날짜 포함해야함, 언제까지 해야함...

라벨에서 어떤 문제인지 라벨링을 할 수 있다
리드미 --> documentation(여러개 체크하거나 수정으로 뺼 수 있음0
assigness = (팀장이)누가 해야하는지 담당자 설정 가능
--> Create 만들면 이슈 생성

이슈 생김 = open / 이슈 해결 = closed

git branch docs/readme
git switch docs/readme
-->브랜치 만들어주는 게 좋다
git push origin docs/readme 


git status
git add README.md
git commit -m "Update dates"
해서 커밋해줘야함

깃허브에서 code -> docs readme branch로 바꾸면 수정된 것 볼 수 있다

oriogin/docs/redme를 origin./main에 넣을때는 'Pull request' 해야 합칠 수 있음, 팀장이 code review 후 합치거나 수정 요구(팀장님께 보고서 보여드리듯이

compare and pull request 녹색 버튼



fix: #1 - 이게 1이슈해결하는 코드라는 걸 밝힘 그리고 create 버튼 누르기

submit review 부분 다시보기 1109 수정해주세요~

LGTM looking good to me

검토해주세요 하고 계속 수정하면 안 된다 --> 준비가 안 됨, 다 하고 올리기

풀과 클론은 다름 git clone은 원격저장소에 있는 레포지토리를 처음 내 로컬에 동기화시킬 떄 사용!!


새 직원 오면 git clon (내가 클론 하고싶은 저장소 웹주소) 주면 된다

cd .. 위폴더로 가기
mkdir clone
cd clone

git log(그동안 fastapi에서 작업한 내용 다 있음)
git log --oneline(한줄로 만들기)

git push: 로컬->원격 업로드
 git pull 원격->로컬다운로드(fetch+merge),변경된 커밋을 가져옴
git clone: 원격-> 로컬다운로드(전체코드 동기화)
클론은 처음 한 번만 하고 이후로는 풀만 하면 된다

깃허브에서 Fork 기능
Git fork: 다른사람 원격을 내 원격으로 복제
게임에서의 프리서버(그 버전까지의 코드 가져와서 다른길로 독자적으로 개발), 이것 말고도 아카이빙의 목적도 있다

ai에게 깃세팅 해달라고 하면 좋다

-------------------------------------------------------------

HTML/CSS

박스표시 - extension (예: 파이썬 하고 싶을 때 원하는 것 추가로 설치)

live Pre preview 설치

HTML hypertext markup languagge 화념에 그려주는 언어
웹 페이지의 구조를 정의하는 언어
글의 제목, 문단, 이미지, 링크 같으 ㄴ웹 페이지의 뼈대를 만드는 역할

웹과 html
서버가 html문서를 만들어서 브라우저에 전달
브라우저는 html을 읽고 화면의 기본구조를 그림
서버-->????????????????

Html 기본 구조
Html 문서는 항상 일정한 기본 틀을 가짐
Tag들의 조합으로 구성
- 태그는 <태그이름> 형태로 작성
- 각 태그마다 요소의 의미와 역할을 가짐
- 대부분의 태그는 여는 태그와 닫는 태그(</>)로 이루어짐

예:
<h1>제목</h1>
<p>문단 내용 </p>

Html 기본구조

태그안에 다른 태그가 들어갈 수 있으며, 이런 중첩 구조로 문서의 계층이 만들어짐
예":
<body> --> 부모 태그
 <h1>제목</h1> -->자식(형제)
 <p>내용</p>    -->형제
</body>


curl example.com 시 html 출력
html을 렌더링(웹에 표시되게 만듬)(브라우저-그림판, 화면에 표시되게 레시피를 주는 것)

웹브라우저
-사용자 대신 http 요청(get) 주소창에 주소 쓰는 것
- html 랜더링

doctype = 문서타입

<html>치면 자동으로 닫아지는 태그도 뜬다(안 되면 탭 눌러보기)
안되면 톱니 - emmet 검색 show abbreviation suggestion 체크확인
show preview(확장파일한거) 하면 오른쪽에 보인다

reveal in explorer 후 연결프로그램-크롬으로 열면 크롬으로 열림
! 치면 기본구조를 자동오로 완성
lang="en" 속성이 들어있으면 그 문서가 어떤 문서인줄 알 수 있어 크롬에서 자동번역 지원(없으면 못함)
charset = "UTF-8" 글씨 깨지던 원인
width = 페이지 너비 initial scale = 기본 사이즈 사용

 Hello, HTML
 Hello, HTML
 Hello, HTML 써도 한줄로 표현(모두 한 덩어리로 인식)
줄바꿈도 태그로 표현해야햠
<p>로 한다면 문단은 한줄 띄기 때문에 한칸씩 띄어진다
<h1> --> <h2> 6까지 있으며 숫자가 커질 수록 글씨 크기는 줄어듦
<hr> horizontal line = 가로선으로 나눌 수 있음. 세로선은 없음!

htlml 에는 두가 지 리스트가 있음
오더드 리스트 언오더드리스트
<ul></ul> 부모
<li>Apple</li> 자식(쇼핑 리스트)
<ol> 은 앞에 순서123 붙여줌

<ol type="I"> 로마숫자로 바꿀 수 있음 (예:  A,  a ...) = attribute


Table 태그
행(row record)

이미지 태그
<img src="" alt= "">
unsplash 에서 새탭에서 이미지 열기
열(column, field)
테이블 위table header

src=소스, 인터넷, 컴퓨터 파일 모두 가능\
alt= 대체: 이미지 못 찾았을때 표시해두면 사진이 있는데 못적었다는 걸 대체텍스트로 알려줄 수 있다

앵커 태그
<body>
    <a href="https://www.google.com">구글</a>로 이동 <a href="">야호~</a>
</body>

폼태그
사용자로부터 뭔가를 입력할 수 있게함
placeholder 자리 맡음(회색글씨)
--> 이메일 예시 적어둘 수 있다

 <input type="emil" placeholder="이메일 입력"> 이메일 쓸때는 type을 email로 하면 @가 있나 없나 검사해줌

<input type="password" placeholder="비밀번호 입력">(글씨를 가려줌)
        <button>입력</button>
        <input type="search" placeholder="검색어 입력"> 칸을 비워줌(왜 있는 기능인지 모름)
        <button>입력</button>

<form action="https://google.com/search">
        <input type="search" name="q"placeholder="검색어 입력"> --> 검색시 구글검색 데이터가 나옴
form: 데이터를 입력받는 HTML 태그(요소)
--> 쿼리 파라미터
action = 구글닷컴/search

GET https://google.com/search?q=... 랑 대치되는 기능

Post(=create)
로도 할 수 있다
회원가입, 게시물 생성, 채팅 생성