#Repository

---
##.gitignore
- 보안상 민감한 정보를 담은 파일을 **배제**할 수 있다.
- git에 commit/history 관리를 하고 싶지 않은 파일에 대해 따로 지정한 것
```
파일명.gitignore
ex) abc.txt.gitignore
```
---
##Git Log
버전마다 차이를 보여준다.
- 통계정보 조회 가능
```
git log --stat
```
- 한줄에 이쁘게 정보 출력
``` 
git log --pretty=oneline
```
---
##Git checkout
git log의 각 코드는 해당상태의 **주소**를 의미한다.
-> 이 코드의 상태로 해당상태로 돌아갈수 있음.
```
git checkout 
앞코드8자리
```
---
##Git Branch
- 갈래 - 분할된 작업 수행
- 원래 소스코드를 유지하면서 여러 시나리오 시도할때
```
git branch #현재 생성된 브랜치 확인
``` 

```
git branch branch_name #새로운 branch 생성
```
```
git switch branch_name #해당 브랜치로 이동
```
```
git branch -d (삭제할 브랜치명) #브랜치 삭제
```
```
git branch -m(기존 브랜치명)(새 브랜치명) #브랜치 이름 바꾸기
```

###Branch 합치기
####1. Merge
- 흔적을 남김
- 브랜치 사용내역들 남겨둘 필요 있으면 
```
git merge brnach_name #Head 기준으로 브랜치 합치기
```
```
git merge --abort #충돌해결
```
####2. Rebase
- 깔끔하게 한줄의 히스토리로
- 협업엔 딱히..