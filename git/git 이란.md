# git 이란?

 세계적으로 가장 많이 사용하고 있는 버전 관리 프로그램

 ## git 시작 방법
 git 설치 후 git에게 자신이 누구인지 알려줘야한다.
 ```git
 git config --global user.email "baesunghoon81@gmail.com
 git config --global user.name "baesunghoon"
 ```

 - `git` : git을 사용하는 명령어
 - `config` : git에 설정을 저장하겠다는 의미
 - `--global` : git이 관리하는 프로젝트에 상관없이 사용한다는 의미
 - `user.email` : git을 사용하는 사용자의 이메일 설정
 - `user.name` : git을 사용하는 사용자의 이름 설정

 1. git으로 관리하고자 하는 프로젝트를 터미널로 열어서 `git init` 작성
 2. `git status` 명령어를 통해서 정상적으로 작동됐는지 확인

 - `git init` : git을 이용해 현재 폴더를 git으로 관리하기 시작
 - `git status` : 현재 프로젝트의 상태를 보여준다. 현재 버전이 무엇인지, 원본과 얼만큼 달라졌는지, 어떤 변경사항을 기록할 것인지 등

 3. 숨김 폴더를 확인해보면 .git 폴더가 생겼을 것이다. 이 .git 폴더는 git 저장소라고 부르고, 이 폴더가 없어진다면 더이상 git의 기능을 사용할 수 없게 된다.



 



