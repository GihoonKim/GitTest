# GitTest

PlayGround for Git function Test

1. git status
   Working Directory와 Staging Area 의 상태를 보여줌.

   "file"을 수정하고 git status를 하면 changes not staged for commit이 있음.

2. git add "file"

    Working Directory에 있는 file을 Staging Area로 보내주는 역할

   이 명령 이후, git status를 진행하면 changes to be committed가 있음.

3. git commit -m "blablabla"
   
   Staging Area에 있는 파일들을 git repository (local) 로 보내줌. 
   -m option은 comment 남겨주기 위함.

