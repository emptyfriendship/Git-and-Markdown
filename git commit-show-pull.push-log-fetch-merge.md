# git commit

버전은 의미 있는 변화를 뜻하며, 작업이 완결된 상태이어야 합니다.

그리고 이렇게 의미 있는 변화에 대해 기록하는 것이 바로 <code>commit</code>입니다.

<br>

# Repository에 commit

     $ git commit -m "feat: README.md update"

-m 은 메세지의 약자이고, 뒤에 ""안에 공유할 메시지 내용을 적어주시면 됩니다.


<br>

# 특정 commit 정보 확인

commit id의 정보 및 수정 내용을 보여줍니다.

commit id는 7자리까지만 입력해도 됩니다.

     $ git show <commit id>

<br>

# 최신 commit 정보 확인

git show는 가장 최신 commit의 정보를 출력합니다.
 
    $ git show

HEAD는 가장 최신 commit을 가리키기 때문에, 아래와 같이 입력해도 됩니다.

    $ git show HEAD

<br>

# 최신 바로 이전 commit 정보 확인

HEAD^는 가장 최신 commit의 이전 commit을 가리킵니다. HEAD^^^은 최신 commit의 3개 전의 commit을 가리킵니다.

    $ git show HEAD^

HEAD~1은 HEAD^과 동일한 의미입니다. HEAD~3은 HEAD^^^과 동일한 의미가 됩니다.

    $ git show HEAD^^^
    
    $ git show HEAD~3

<br>

# 원격 저장소에 push, 업데이트 된 내용은 pull

내 local 디렉토리로 부터 원격저장소(Remote repository)로 보내기 위해서는 <code>push</code> 명령어를 사용합니다.

그 전에 원격 저장소와 내 로컬을 연결해야 합니다.

    $ git remote add origin (원격 저장소 github URL)

 __push__

    $ git push origin master
    
origin이라는 원격저장소의 master 브랜치에 푸쉬합니다

 __pull__
 
 또한 다른 사람이 원격 저장소(Remote repository)에 업데이트한 파일이 있을 때,     
 원격저장소와 내 로컬저장소의 상태를 동일하게 만들기 위해 <code>pull</code>을 이용합니다.
    
    $ git pull
    
 <br>
 
 # 커밋 이력 확인
    
    $ git log
    
또는

한 줄로 요약해서 보고 싶은 경우

    $ git log --oneline
    
    
# git clone 명령어

     $ git clone [REPO_URL] [DIR]
     
클론한 저장소의 원격 저장소 위치 확인하기
    
    $ git remote -v
    
특정 브랜치(태그)만 클론하기    

    $ git clone --branch [TAG] [REPO_URL]
    
    
 #  fetch
    
 원격저장소 코드를 수동으로 내려받는 작업
 
    $ git fetch 원격저장소URL
    
 # merge  
    
 fetch 상태에서 merge를 통해 병합할 수 있다 
 
    $ git merge 원격저장소별칭 or 브랜치
