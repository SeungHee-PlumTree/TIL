###Repository

---
###.gitignore
- 보안상 민감한 정보를 담은 파일을 배제할 수 있다.
- git에 commit/history 관리를 하고 싶지 않은 파일에 대해 따로 지정한 것
```
파일명.gitignore
ex) abc.txt.gitignore
```
---
##Git Log
버전마다 차이를 보여준다.
```
git log --stat #통계정보 조회 가능
git log --pretty=oneline #한줄에 이쁘게 정보 출력
```
---
##Git checkout
git log의 각 코드는 해당상태의 주소를 의미한다 -> 이 코드의 상태로 해당상태로 돌아갈수 있음.
```
git checkout 
앞코드8자리
```
---
##Git BRANCH
*갈래 - 분할된 작업 수행
*원래 소스코드를 유지하면서 여러 시나리오 시도할때
```
git branch #현재 생성된 브랜치
``` 

```
git branch branch_name #새로운 branch 생성
```
```
git checkout branch_name #해당 브랜치로 변경
```
---
##Merge
```
git merge brnach_name #Head 기준으로 브랜치 합치기
```
  