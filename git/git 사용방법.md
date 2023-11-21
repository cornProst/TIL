 ## 프로젝트에 파일 추가
  파일을 생성하고 `git status` 명령어로 현재 상태를 확인해보면, `Untracked files:` 항목에 방금 생성한 파일이 올라가게 된다. 이 뜻은 git이 관리하고 있지 않은 파일이다.

  이 상태에서 `git add 파일제목`을 입력하면 git이 관리하는 파일로 변하게 된다.

 - `git add <파일 이름>` : 프로젝트에 추가할 파일 선정
 - `git add --all` : 모든 변경사항 파일 추가
 - `git commit -m "<커밋 메세지>` : 선정된 파일들이 왜 추가되었는지 알기위한 이유와 함께 git에 추가하는 명령어

 git에서 관리되는 프로젝트의 파일을 세 가지 상태로 정리할 수 있다.
 
 1. git에 추가되지 않은 상태
 2. git에 추가할 준비 상태 (git add를 진행한 상태)
 3. git에 추가된 상태 (git commit을 진행한 상태)

 ## git의 관리 대상에서 제외하기
 개발자는 협업을 하기에 각자의 컴퓨터가 사용하는 OS나 설정이 다를 수 있기에 이러한 파일들은 git이 관리하는 파일에서 제외시켜주는 것이 좋다.

 `.gitignore` 파일은 git이 버전관리를 하면서 확인하도록 설정되어있는 파일로, 여기에 기록된 파일 또는 폴더는 git이 추가하지 않는다.

 1. 폴더에 .gitignore 파일 생성
 2. do-not-add 파일 생성
 3. .gitignore 내부에 do-not-add라고 작성하면 git status로 확인해도 해당 파일 확인 할 수 없음

 ## git - restore, reset
 git은 변동사항, 작업이력을 commit 단위로 작성한다. 실수로 commit했거나 되돌리고 싶을 때 restore, reset명령어를 사용한다.

 `git restore --staged <파일명>` : add한 파일 취소
 `git reset <commit id>` : 해당 commit id까지 프로젝트의 상태가 되돌아감

 