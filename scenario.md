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