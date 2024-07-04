## 깃허브로 다른 사람과 공동 작업하기 

- git hub 서버, 공동작업하는 로컬 a, b 끼리 내용이 같게 관리 필요

- *충돌이 일어날 경우...*
    - **push & pull 로 버전을 비교, 관리**
        - current change : 내가 수정한 결과를 반영
        - incoming change : 내려받은 결과를 반영 (상대가 수정한 내용)
        - accept both change : 둘 다 반영?

### branch 개념
![branch_이해하기](https://velog.velcdn.com/images%2Fdiduya%2Fpost%2Faa5094be-7a50-4c32-8584-f4746a57e669%2Fgit-flow_overall_graph.png)

- 브랜치 생성 명령
    - git branch -c (branch명)
- 브랜치 이동 명령
    - git switch (branch명)
- 브랜치 삭제
    - git branch -d (branch명)
- 브랜치 합병
    - git merge (브랜치명)
        - master에서 실행한다 : 여러명 작업을 위해 각자의 브랜치에서 일하다가 master에 병합해야한다.
	- 충돌이 일어날 경우.....
        - git push 시 오류 (충돌) <- esc > shift + : 다시 push
	    - merge시 구문 통일에 유념?

### 코드에 기여하기 (Contribution)
- fork(복제) : 다른 사람의 깃의 사본 만들기
- 소통, 또 하나의 SNS