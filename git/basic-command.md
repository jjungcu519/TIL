# Git command

> git 기본 명령어를 정리해봅시당

## init
- 현재 위치(pwd)에 `.git` 폴더를 생성 (앞에 .이 붙으면 숨겨진 폴더라는 뜻) 추적

```bash
git init
```

> git이란? : 분산 버전 관리 시스템 (리비전?)

## add
- working directory 에서 staging area 로 업로드 하는 과정 (추적 가능하게 만드는 과정 Untracked -> index tracked)
![i1](https://git-scm.com/book/en/v2/images/areas.png)

```bash
git add .
```

## status
- 현재 git 상태 확인 명령어
```bash
git status
```

## commit
- staging area에 올라간 내용을 스냅샷 찍는 과정
```bash
git commit -m "first commit"
```

> -m 옵션을 통해 메세지를 관리한다.


***add commit의 수레바퀴가 돌아간다~***