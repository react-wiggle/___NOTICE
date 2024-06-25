# notice
브랜치 보호 규칙

# 깃 허브 적용 규칙
1. fetch 및 pull : 코드 수정 전 최신 코드를 로컬로 받기
2. commit : 작업 완료 후 코드를 수정하고 commit
3. fetch 및 pull : 다시 원격 저장소에서 최신 변경 사항을 가져온다.
4. 충돌 해결 : git pull 중에 충돌이 발생하면, 충돌을 해결하고 commit 한다.
5. Push : 로컬 변경 사항을 원격 저장소(git)에 푸시한다.
6. Pull Request : 팀장에게 merge 요청 

## 이 순서를 권장하는 이유
1. 충돌 최소화 : 작업 후 먼저 'pull'을 하여 최신 변경 사항을 가져오면, git에 있는 변경사항과 로컬 변경사항을 병합할 수 있다.
                이때 충돌이 발생하면 로컬 환경에서 해결할 수 있어, 푸시할 때 다른 팀원의 작업에 영향을 주지 않는다.
2. 코드 일관성 유지 : 최신 코드를 로컬에 반영한 후 푸시하면, git과의 일관성을 유지할 수 있다.
                     이는 다른 팀원이 'pull'할때 예상치 못한 충돌을 피하는데 도움이 된다. 

# Pull Request 만들기
1) fork
① 팀장의 Repository에 접속한 후 Fork 버튼을 누른다.
 
② Create a fork를 누른다.
 
③ 자신의 Repository에서 fork로 생성된 새로운 저장소를 확인할 수 있다.
 
2) Clone, Remote
① fork로 생성한 본인의 Repository에서 Code 버튼을 눌러 HTTPS 주소를 복사한다.
코드를 수정한다.

④ commit을 실행한 후 본인의 Repositroy로 수정한 코드를 push한다. (가끔 push 하는 브랜치의 이름이 main으로 되어 있어 push가 안될 수도 있는데, 이 때는 다른 이름으로 바꿔주면 된다.)
 
⑤ fork된 Repository에서 파란색 글씨로 적힌 1 commit ahead를 클릭한다.
 
⑥ Create pull request를 클릭한다.
 
⑦ 원하는 메시지를 입력한 후 Create pull request를 클릭한다.
 
⑧ pull request 생성이 완료되면 우측에 Reviewrs라는 창이 보이는데, 톱니바퀴 버튼을 눌러 팀원들을 reviewer로 설정한다.
 
⑨ 팀장은 본인의 Repository의 Pull request 버튼을 클릭해 pull request를 확인할 수 있다. 코드 변경 내용을 확인하고 Merge 여부를 결정한다.
 
⑩ 변경 사항이 적용되면, 최근 코드를 pull하여 동기화를 진행한 후 협업을 이어간다.

#.gitignore 파일
### 깃이나 외부에 배포할 때 제외할 파일 기재
협업할 때 필요한 파일이 공유가 안될 수 있어 절대 수정 금지
