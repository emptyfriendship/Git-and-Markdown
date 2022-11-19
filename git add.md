# git add 기본 개념/사용법

 <code>git add</code>는 작업 디렉토리(working directory) 상의 변경 내용을 스테이징 영역(staging area)에     
 추가하기 위해서 사용하는 Git 명령어입니다.

<br>

# git commit vs. git add

<code>git add</code> 명령어는 다음 변경(commit)을 기록할 때까지 변경분을 모아놓기 위해서 사용합니다. 

따라서, <code>git commit</code> 명령어를 통해 명시적으로 기록을 남기기 전까지는 아무리 <code>git add</code> 명령어를 많이 실행해도     

Git 저장소의 변경 이력에는 어떤 영향도 주지 않습니다.    

<br>

# git status

<code>git add</code> 명령어를 사용할 때, 항상 함께 사용하게 되는 명령어가 <code>git status</code> 입니다. 

<code>git status</code> 명령어는 작업 디렉토리(working directory)와 스테이징 영역(staging area)의 상태를 확인하기 위해서 사용합니다.

<br>

# 기본 사용법

첫 번째, 작업 디렉토리의 변경 내용의 일부만 스테이징 영역에 넘기고 싶을 때는     
수정한 파일이나 디렉토리의 경로를 인자로 넘깁니다.

     $ git add <파일/디렉토리 경로>
     
두 번째, 현재 디렉토리의 모든 변경 내용을 스테이징 영역으로 넘기고 싶을 때는, .을 인자로 넘김니다.      
      
     $ git add .
      
세 번째, 작업 디렉토리 내의 모든 변경 내용을 몽땅 스테이징 영역으로 넘기고 싶을 때는, -A 옵션을 사용합니다.   

    $ git add -A
      
      
      
      
      
      
      
      
      
      
      
      
