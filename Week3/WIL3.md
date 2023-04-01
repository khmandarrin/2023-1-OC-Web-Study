
Git이 관리하는 파일의 4가지 상태
> untracked, unmodified(추적 중인 파일이 변경 변경되지 않은 상태), modified(추적 중인 파일이 변경 된 상태), staged

working directory > 작업 공간, 코드 변화 추적, 일정 갯수의 변화 저장
staging area > 파일의 변화들을 쌓아놓는 공간
local repository > 내 컴퓨터의 저장소
remote repository > 데이터를 공유할 수 있는 공통 외부 저장소

Clone 
> 깃허브 Repository에 있는 파일을 내 로컬 컴퓨터로 복사해오는 작업

repository 생성하고 local에 복사
> 깃허브에서 repository 카테고리 - New 클릭
> 연동할 저장소 Code에서 url복사하여 clone

명령어 
git init //repository 생성, 추적 및 관리
git clone [REPO_URL] [DIR] // repository를 local에 복사
git status // 파일 변경, 추가 사항 확인
git add "파일이름" // 파일을 staging area에 추가
git commit -m "Commit message" //commit 명령어
git push <remote> <branch> // push 명령어
    ㄴex) git push -u origin master // master 브랜치로 push
    기본적으로 원격저장소는 origin, 브랜치는 현재 작업하고 있는 브랜치