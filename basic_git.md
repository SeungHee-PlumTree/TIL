#Git 
---

1. *초기화*
```
git init
```

2. *추가할 파일 더하기*
```
git add .
```
* **.(점)** 은 모든 파일임. 선택적으로 올리고 싶으면 add 뒤에 파일명 붙이기. (ex. git add prac2)

3. 상태 확인 (선택사항)
```
git status
```

4. 히스토리 만들기
```
git commit -m "first commit"
```
* -m 은 메세지의 준말로 뒤에 "" 안에 주고싶은 히스토리 이름을 주면 됨( first, second, ~)

5. Github repository랑 내 로컬 프로젝트랑 연결
```
git remote add origin https:/github.com/SeungHee-PlumTree/~
```
* github 에서 복사해서 붙이기

6. 잘 연결되었는지 확인(선택사항)
```
git remote -v
```
* 내가 연결한 주소값이 뜨면 성공임

7. Github로 올리기
```
git push -u origin master/main
```
* master 자리에는 Branch 이름이 들어가면 됨. 


#Github에 계속 업데이트 하는 법
---
1. 추가할 파일 더하기
```
git add . 
```

2. 히스토리 만들기
```
git commit -m ""
```

3. Github로 올리기
```
git push origin main
```
내 컴퓨터에 소스코드를 업데이트 하고 싶으면 **세개의 스텝**만 반복하면 됨