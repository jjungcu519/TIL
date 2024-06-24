# LINUX command : 기본 명령어 정리

* `pwd` (print working directory)
    - 현재 작업중인 경로를 표시
* `clear` (`ctrl + l`)
    - 터미널 창을 지워주는 명령어
* `ls`
    - 현재 폴더에 있는 파일, 폴더 목록 표시
        - 파란색 : 폴더 / 하얀색 : 파일
    - `-a (option)` : 숨겨진 목록까지 표시
        - 앞에 .이 붙으면 숨겨진 폴더라는 뜻
- `mkdir {directory_name}`
    - 폴더 생성 명령어 (New folder)
    - **directory_name : 폴더이름**
        - ex. mkdir test 
- `touch {file_name}`
    - 파일 생성 명령어
    - **file_name : 파일이름**
        - ex. touch a.txt
- `rm {name}`
    - 파일 삭제 ex.rm aa.text
        - *cf. tab 자동완성 기능 활용*
    - `-r` : 폴더 삭제를 위해 달아주는 옵션
        -   ex.rm -r test
- `cd` (change directory)
    - 경로이동 명령어
        - `cd ~` : 태초마을 (home directory)
        - `cd .` : 현 위치 찍어줌
        - `cd ..` : 상위폴더로 이동
        - `cd {directory_name}` : 해당 폴더로 이동
            - ex. cd Desktop/DMF/linux/
    
