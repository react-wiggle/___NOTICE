# notice
브랜치 보호 규칙

# 깃 허브 적용 규칙
1. 작업 시작 전 fetch 업데이트
2. pull 받을게 있으면 pull 받기
3. 작업 후 commit
4. 다시 fetch하여 pull 받을게 있으면 pull 받기
5. pull 받은 코드와 작업한 코드가 conflict 되는 부분이 있는지 확인
6. 확인되었으면 push 한 후 Pull Request 요청하기

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
