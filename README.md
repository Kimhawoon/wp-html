# HTML 내용 정리
    HTML-> 구조 및 내용 구성
    CSS-> 디자인 구성
## HTML 기본용어
    -태그: 객체 생성 (쌍, 단독) <h1></h1>, <br>
    -요소: 태그로 만들어진 객체
    -속성: 태그에 정보 추가 <h1 class="~"> (여러개 가능)
    -주석: 코드 부연 설명, 앞으로 해야할 일 메모 <!-- ~ -->
----
## HTML5 페이지 구조
    <! doctype html> (HTML 버전 명시)
    <html lang="ko"> (시작태그, 언어)
    <head> ~ </head>
    <body> ~ </body> (사용자에게 보여지는 부분)
    </html> (끝태그)

    <head>: 페이지 정보제공
        <title> ~ </title> 제목
        meta: 추가 정보 전달
        script: 스크립트 추가
        link: 다른 파일 추가
        style: 스타일시트 코드 추가
        base: 기본 경로 지정

    *주의할점
    <시작></끝> 엇갈리지 말아야함!!    
----
## 기본태그 
    -글자 관련 태그 <h1~h6, 숫자가 작을수록 글자가 큼> 
    -본문 관련 태그 <p, br, hr>
    -글자 형태 관련 태그 <b, i, small, sub, sup, ins, del>
    -앵커 태그 <a href=""></a>
----

## 목록 관련 태그
    ul: 순서 없는 목록 
    ol: 순서 있는 목록
    li: ul or li 중 목록 아이탬 나타내기
----
## 테이블 태그
    caption: 표의 제목
    thead: 표의 헤더
    tbody: 표의 몸체
    tfoot: 표의 푸터
    tr: 표의 행
    th: 표의 제목 셀 생성 (tr 내부 칸)
    td: 표의 데이터 셀 생성 (tr 내부)
    border: 표 라인 생성

    (속성) rowspan="" 위아래 합치기
           colspan="" 양옆 합치기
----
## 공간 분할 태그
    inline: 옆으로 나열 <a, 글자 형태 관련 태그>
    block: 위에서 아래로 쌓임 <p, 제목 태그>

    공간은 레이아웃을 잡기 위해 생성
    <div> ~ </div>: block 형식 공간 생성
    <span> ~ </span>: inline 형식 공간 생성
    semantic 구조
       *태그에 의미가 존재함 (div와의 차이점)
        header 위
        nav 네비게이션
        aside 옆
        section 중심내용 (article 모음)
        aticle 주요 글
        footer 아래

----

## 이미지 태그
    img
    (속성)   src: 이미지 주소 지정
             alt: 이미지 로드 할 수 없을 때 설명글
             width: 이미지 너비
             height: 이미지 높이

----
## 오디오 태그
    audio
    (속성) src: 경로 저장
         preload: 로드 범위 지정
         autoplay: 자동재생
         loop: 반복재생
         controls: 재생 도구 표시
    -source: 브라우저 버전마다 음악 파일 지원 형식이 다를 때 해결

----

## 비디오 태그
    video
        (속성) src: 경로 저장
               poster: 동영상 준비 시 표시할 이미지 파일 경로 지정
               preload: 로드 범위 지정
               autoplay: 자동재생
               loop: 반복재생
               controls: 재생 도구 표시
               width: 너비
               height: 높이

----

## 입력 양식 태그
    사용자로부터 데이터 입력 받기
    form 태그들 배치
        action: 데이터 위치 지정
        method: 데이터 전달 방식 지정
        type: 입력 양식의 종류 결정 (button, checkbox, file, password, radio, reset
                                     submit, text, email, tel, number, date ...)
    input 데이터 입력
        name: 서버 구분용 이름
        placeholder: 사용자 입력 안할 시 안내글
        disabled: 비활성화
        readonly: 읽기만
        value: 입력 양식의 값
    textarea
        cols: 태그의 너비 지정 (한 줄에 글자 몇개?)
        rows: 태그의 높이 지정 (라인 수)
        nam:e 이름
        placeholder: 안내글
        disabled: 비활성화
    select: 선택 양식을 생성
        optgroup: 옵션을 그룹화 (태그)
        option: 선택할 수 있는 옵션 생성 (태그)
        (속성) name 이름
               multiple 중복선택
               disabled 비활성화

    label 설명을 넣기 위함 (*아이디: ____)
        for 입력 양식의 id 속성 값 (모든 곳에 사용, 중복 X)
    fieldset 그룹나누기
    legend 그룹이름