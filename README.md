## 작업 시나리오

다음과 같은 순서로 작업을 진행하였습니다. 

1. Fast-Forward merge : 혼자 개발하는 상황을 가정하여 jin2 branch를 개설한 후 html 파일 내용을 수정하여 main에서 merge 했습니다.
(jin2 commit) 

2. 3-way-merge : 각각의 브랜치를 만들어서 각자 이름의 html 파일을 생성한 뒤, main.html 파일 내용을 수정한 뒤, main에서 merge하고 
충돌을 해결했습니다. (1차 충돌 수정 commit , 충돌 2차 수정 commit)

3. rebase : main 브랜치에서 jaehee.html 파일 수정 후 commit , jaehee 브랜치로 이동 후 jaehee.txt 파일 수정 후 rebase merge를 
진행했습니다. (main edit commit for rebase, jaehee branch commit for rebase commit)

4. squash : SeYeong 브랜치에서 h4,h5,h6 태그 수정에 관한 3개의 commit을 생성한 후, 하나의 h태그 수정 commit으로 만들면서 merge를
진행했습니다. (SeYeong html h태그 추가 commit)  


<br>

## branching/merge  가이드

/{name} 으로 branch를 생성하여 각자 작업한 후 main에서 merge하는 전략을 사용했습니다.

저희 팀이 어떤 상황에서 어떤 merge를 사용하는 것에 대한 전략은 다음과 같이 구상했습니다.

### 1. Rebase
- 내 브랜치 커밋을 다른 브랜치의 최신 커밋 위로 재적용시
- 커밋 히스토리 깔끔하게 하고 추적하기 쉽게 할 때

### 2. squash
- 여러 커밋을 하나로 합침
- 기능 개발이 끝난 브랜치를 하나의 커밋으로 main에 넣을때

### 3. Fast-forward
- main에서 새브랜치를 만들어 작업한 뒤, 충돌없이 바로 병합가능할 시

### 4. 3-way
- 두 브랜치에서 동시 작업하여 커밋이 갈라졌을 시
- 공통 조상 커밋과 두 브랜치의 커밋을 비교해 병합 커밋 생성
