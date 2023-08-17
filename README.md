# git-practice

### Remote Repository(원격)
- Github 온라인에 저장된 리포지토리 --> e.g. google drive, iCloud...

### Local Repository(로컬)
- 작업 중인 PC에 저장된 리포지토리 --> e.g. 내 PC의 프로젝트 폴더

### Remote - Local 연결 확인 방법
1. 프로젝트 폴더 오른쪽 마우스-Git Bash Here
2. git remote -v
    - fetch, push url 2줄이 나온다면 정상 연결 상태
    - 연결이 되지 않았을 경우
      - git remote add origin https://github.com/devyuwon/git-practice.git

### Branch pull
- git에 업로드 된 최신 코드를 받아 오는 과정
- 메뉴-Git-pull-git pull origin main

### Git Branch 생성
- 메뉴-Git-New Branch..
    - 브랜치명은 본인의 이름(영문)으로 생성
    - Checkout Branch 체크
      - Checkout: 작업할 Branch를 변경하는 git 명령어

### 새로운 Branch에서 작업하는 방법
- 메뉴-Git-Branches-Local Branch-본인이 생성한 Branch-Checkout

### 새로운 Branch에 commit, push
1. activity_main.xml 내 TextView 문구를 본인 이름으로 변경
2. commit
    - commit convention -> Design: activity_main TextView 문구 수정
3. push
    - 생성한 Branch가 선택되어 있는지 확인 후 push

### Pull Request(PR)
- 작업한 Branch 코드가 Error 없이 정상적으로 작동하는 경우 상위 Branch(e.g. main or dev)에 merge(합병)하는 과정
- 바로 merge하는 방법도 있지만, Pull Request로 merge하면 코드 충돌을 최소화 할 수 있다.
- Pull Request는 Repository의 관리자만 승인할 수 있다.
