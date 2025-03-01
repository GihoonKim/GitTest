# GitTest

PlayGround for Git function Test

1. git status
   Working Directory와 Staging Area 의 상태를 보여줌.
   Remote branch에 비해 몇 commit 앞서 있는지도 같이 나옴.

   "file"을 수정하고 git status를 하면 changes not staged for commit이 있음.

2. git add "file"

    Working Directory에 있는 file을 Staging Area로 보내주는 역할

   이 명령 이후, git status를 진행하면 changes to be committed가 있음.

3. git commit -m "blablabla"
   
   Staging Area에 있는 파일들을 git repository (local) 로 보내줌. 
   -m option은 comment 남겨주기 위함.

   이러면 새로운 HEAD가 생기고 "file"은 새로운 HEAD에서 unmodified 파일로 변경됨.

4. git log --oneline

    git commit 내역을 보고 싶을 때. 

5. git checkout <커밋해시>
    이전 commit된 곳으로 일시적!!으로 돌아가고 싶을 때! (이 상태는 Detached HEAD 모드이므로, 이후 변경 사항이 새로운 브랜치로 연결되지 않음)

    다시 최신으로 돌아가고 싶다면 git checkout "branch" 혹은 git checkout - 입력

6. git reset --soft <커밋해시>
    hard 옵션은 변경 사항이 완전히 사라지기 때문에 주의해야 합니다.
    soft 옵션은 해당 커밋으로 이동하되, 변경 사항은 staging area에 남겨 놓습니다. mixed는 변경 사항을 워킹 디렉토리로 이동
    <커밋해시> 대신 HEAD~num 옵션으로 num 단계 이전 커밋으로 이동 가능합니다.


