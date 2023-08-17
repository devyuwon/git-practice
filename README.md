# git-practice


### Remote Repository(원격)
---
- Github 온라인에 저장된 리포지토리 --> e.g. google drive, iCloud...


### Local Repository(로컬)
---  
- 작업 중인 PC에 저장된 리포지토리 --> e.g. 내 PC의 프로젝트 폴더


### Remote - Local 내려받기 --> `clone`
---  
1. Repository 초록색 Code 버튼 클릭
2. HTTPS URL 복사
3. 메뉴-Git-Clone
    - URL: 복사한 URL 입력
    - Directory: 프로젝트 경로 설정


### Remote - Local 연결 확인 방법
---  
1. 프로젝트 폴더 오른쪽 마우스-`Git Bash Here`
2. `git remote -v`
    - fetch, push URL 2줄이 나온다면 정상 연결 상태
    - 연결이 되지 않았을 경우
        - `git remote add origin https://github.com/devyuwon/git-practice.git`


### Git Branch 생성
---  
1. 메뉴-Git-New Branch..
    - 브랜치명은 본인의 이름(영문)으로 생성
2. Checkout Branch 체크
    - `Checkout`: 작업할 Branch를 변경하는 git 명령어


### 새로운 Branch에서 작업하는 방법
---  
- 메뉴-Git-Branches-Local Branch-본인이 생성한 Branch-Checkout


### 새로운 Branch에 commit, push
---  
1. `activity_main.xml` 내 textView 문구를 본인 이름으로 변경
2. `commit`
    - commit convention -> Design: activity_main TextView 문구 수정
3. `push`
    - 생성한 Branch가 선택되어 있는지 확인 후 push


### Branch pull
---
- git에 업로드 되어 있는 최신 코드를 받아 오는 과정
    1. `activity_main.xml`에서 `textView2` 삭제
    2. 메뉴-Git-pull-git pull origin main
    3. `textView2` 복구 여부 확인


### Pull Request(PR)
---  
- 작업한 Branch 코드가 Error 없이 정상적으로 작동하는 경우 상위 Branch(e.g. main or dev)에 merge(합병)하는 과정
- 바로 merge하는 방법도 있지만, Pull Request로 merge하면 코드 충돌을 최소화 할 수 있다.
- Pull Request는 Repository의 관리자만 승인할 수 있다.
