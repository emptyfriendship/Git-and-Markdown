# reset

reset 명령어를 사용하면 지정된 코드로 되돌아감

    $ git reset 옵션 커밋ID
    
  <br>
    
# soft 
 
    $ git reset --soft 커밋ID

soft 옵션은 지정한 커밋 위치로 복귀

복귀하면서 스테이지 영역의 상태도 같이 복귀

<br>

# mixed 

mixed는 reset 명령어의 기본값

    $ git reset --mixed 커밋ID
    
    $ git reset 커밋ID
    
mixed 옵션은 스테이지 상태를 제외하고 복원하기 때문에 커밋을 하려면 add 명령어를 먼저 해야함

# hard

hard 옵션은 리셋되는 복귀 시점의 커밋 상태와 해당 커밋의 워킹 디렉터리까지 모두 되돌림

    $ git reset --hard
    
  <br>
    
# 스테이지 리셋

    $ git reset <파일이름>
    
    $ git reset --mixed HEAD <파일이름>
    
<br>

# revert

리버트는 기존 커밋을 남겨 두고 취소에 대한 새로운 커밋을 생성

    $ git revert HEAD

리버트 지정

깃의 범위 지정 연산자를 이용해 여러 커밋을 리버트 할 수도 있음

    $ git revert 커밋ID .... 커밋ID






    
    
