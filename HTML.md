#HTML
1. 메모장켜서 내용을 입력한 뒤 **파일명.html**로 저장
2. **모든 파일**로 설정 + **인코딩 UTF-8** 로 설정

---
##TAG
#####단어를 강조할때
```
<태그명> 해파리 </태그명>
``` 
-> 나는 **해파리** 이다
<br>~~~~~
<br>
<br>
#####제목을 강조할때
```
<h1> 제목 </h1> # h는 heading의 약자
1,2,3.. 글자 크기 작아짐
```
-> **제목**

---
##속성
#####링크를 넣고 싶을때
{ <태그명> 해파리 </태그명> }

- `<태그명 href="링크"> 해파리 </태그명>` : *해파리* 를 누르면 링크로 이동

- `<태그명 href="링크" target="_blank"> 해파리 </태그명>` : *해파리* 를 누르면 *또 다른 탭* 생성되어 링크로 이동
- `<태그명 href="링크" title="젤리뽕뽕"> 해파리 </태그명>` : *해파리* 에 마우스를 갖다대면 *젤리뽕뽕* 가 나타남
---

##리스트와 태그의 중첩
html 은 줄바꿈을 무시를 하는데! 
- `<li> 해파리 </li>` : 리스트 줄바꿈
```
해파리
물개
가재
```

- `<ul> 해파리 </ul>` : 리스트를 순서가 없는 그룹으로 묶기
- `<ol> 해파리 </ol>` : 리스트를 순서가 있는 그룹으로 묶기
```
1. 해파리
2. 물개
3. 가재
```
- `<title></title>` : 제일 위 제목
- `<meta charset="utf-8">` : 글자 깨졌을때
---
##문서 구조
1. `<html> head, body, ~ </html>` : 가장 바깥에
- `<head> title, meta~ </head>` 
- `<body> 본문 </body>` 
---

##단락 : P
```
<p>~</p>
```
-> 기본적으로 한줄 떨어뜨림 (더 떨어뜨리거나 안 떨어뜨리거나 싶으면 css에서..)

##줄바꿈 : br

```
뒤에다가 <br>
```
1개 : 바로 뛰움 2개: 한줄 뛰움 3개: 두줄 뛰움 ~~~<br><br>
>단락 표현하고 싶으면 p태그를 쓰자

##이미지 : img

`<img src="img.jpg"> `
- 추가 : 폭: width = "100" / 높이: height = "100" /alt = "산 이미지"

`alternative text` : 이미지가 깨졌을때 대안

---

##Table

- **`<table></table>`** : 전체 묶어주기 <-무조건 해줘야함
   
- `border = "1"` : 표 테두리

- `<tr></tr>`: 행 그룹핑
- `<td></td>`: 열/항목 하나씩 묶어주기
- `<thead></thead>` : <th></th> 상단 열 표시
- `<tbody></tbody>`
- `<tfoot></tfoot>` : 맨밑
- `rowspan="2"` : 행 병합
- `colspan="2"` : 열 병합

```ts
example_table

<table border="3">
<thead>
 <tr>
  <th>이름</th> <th>성별</th>
 </tr>
</thead>
<tbody>
 <tr>
  <td>이승희</td><td>여</td>
</tbody>
<tfooot>
 <tr>
  <td colspan="2">AE 승희</td>
 </tr>
<t/foot>
```

---

##Form
사용자가 입력한 정보들을 서버로 전달해주는 것들
- ` form action="링크"` : form 안에 있는 것을 수행하면 링크로 이동한다. 
- `input type =` 
  - `"text"` : 입력
  - `"password"` : 비밀번호처럼 나옴
  - `"submit"` : 제출이라는 버튼
  - `"reset"` : 입력 정보 초기화
  - `"file"` : 파일선택
- `name = " "` : input 이름
- `textarea` : 여러줄 입력 가능한 입력창
  - `cols="50"` : 한줄에 50자
  - `rows="2"` : 두 줄

---

##Form : dropdown list
- `<select>`: 선택리스트
  - `name=""` : select 이름
  - `multiple=""` : 여러개 선택가능(체크박스가 더 좋긴함)
- `<option value ="">` : 선택지

---

##Form : radio, checkbox, label
- `<input type="radio">` : 동그란버튼 생성
  - radio버튼은 name 같은 그룹 내에서 하나 선택되면 하나 해제됨.
- `<input type="checkbox">` : 다중선택 가능한 버튼 생성  
- `<label>Label</label>` : Label이 하나가 됨. - 사용성 높임

---

##Form : Method
- `method=""` : 데이터전송방식
  - `"get"` : URL로 전송
  - `"post"` : 데이터를 숨겨서 전송 <- 보통 이거로 하셈
- `enctype` : 

---

##Font
- `font size=""` : 글자 크기 (기본 3)
- `color = ""` : 글자색깔

---
##Meta
- `인코딩` : 코드들을 컴퓨터에 저장하는거
- `딥코딩` : 저장된걸 꺼내서 화면에 표시하는거

---
##의미론적 태그
- `<article></article>` : 본문
- `<header></header>` :화면 **상단**에 위치하는 사이트나 문서의 전체적인 정보 정의
- `<footer></footer>` : 화면 **하단**에 위치하는 사이트나 문서의 전체적인 정보 정의
- `<nav></nav>` : 문서의 네비게이션 항목 정의
