# Git command: 기본 명령어 정리

## 들어가기에 앞서
![i1](https://git-scm.com/book/en/v2/images/areas.png)
[출처 : 3 stages working tree](https://git-scm.com/book/ko/v2/%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0-Git-%EA%B8%B0%EC%B4%88)

>*cf. 3stage란? modified/staged/commited*


## 0. 깃 관리
- 프로젝트별 (폴더별) git 관리를 진행하는 것을 권장
-ls -a로 .git 파일이 있는지 확인하고 신규 레파지토리 생성
- 관리하지 않는 venv requirements 등은 .git ignore로 관리
    - 2. add 하기 전까지 반드시 .gitignore 파일을 생성해주자. 

## 1. init
- 현재 위치(pwd)에 추적을 위한 `.git` 폴더를 생성
    - .git이 상,하위 폴더에 동시에 존재하면 충돌한다.

```bash
git init
```

> *cf. git이란 분산 버전 관리 시스템의 일종 (.git은 github와 연결을 위한 장치?)*

## 2. add
- **working directory 에서 staging area 로 업로드 하는 과정**
    - 추적 가능하게 만듦. (Untracked -> index tracked)


```bash
git add .
```

## 3. status
- 현재 git 상태를 확인하는 명령어
    - **내용이 modified 되었으면 저장후 add . 진행**
```bash
git status
```

## 4. commit
- staging area에 올라간 내용을 스냅샷 찍는 과정
```bash
git commit -m "first commit"
```

> *cf. -m 옵션을 통해 커밋 메세지를 관리한다.*


## 5. remote add
- 원격저장소의 주소를 저장하는 명령어
    - ex. git remote add origin https://github.com/jjungcu519/trial.git

```bash
git remote add {remote_name} {remote_url}
```

## 6. push
- 원격 저장소로 브랜치를 업로드하는 명령어
    - ex. git push origin master
```bash
git push {remote_name} {branch_name}
```

---
## 정리
- 2는 working directory를 staging area로 만든다.
    - modified 된 내용이 있다면 저장후 다시 add . 하자
- 4는 staging area에 있는 내용을 확정짓는다. (스냅샷)
    - 이 때 stage fixed (변경사항)이 없으면 commit할게 없다고 출력
- 6은 확정지은 내용을 로컬 디렉토리 (깃허브)로 밀어낸다.