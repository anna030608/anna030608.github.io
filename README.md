## Build 과정

### Github Page 만들기
1. 나의 github계정에 anna030608.github.io라는 이름으로 repository 만든다.
2. Remote Repository의 주소를 복사한다.
3. Git Bash를 실행시킨다.
4. "git clone <2번에서 복사한 주소 붙여넣기> <내가 저장할 path 넣기>"를 통해 clone 시킨다.
5. "git branch -M main"을 통해 현재 branch 이름을 master에서 main으로 바꾼다.
6. PAT를 만든다.
7. "git push origin main"을 통해 원격저장소에 반영한다.

### Jekyll 사이트 만들기
1. jekyll 윈도우용으로 다운받는다.
2. "cd <지정한 path>"로 내가 지정한 path로 디렉토리를 이동한다.
3. "jekyll -v"를 통해 jekyll 설치 확인 및 버전을 확인한다.
4. "jekyll new . --force"를 통해 현재 디렉토리에 jekyll을 설치한다.
5. "ls"를 통해 새로 생긴 파일이 있는지 확인한다.
6. "git add *"를 해서 새로운 파일 반영한다.
7. "git commit -m "커밋메세지""를 통해 저장한다.
8. "git push origin main"을 통해 원격저장소에 업로드한다.
9. "bundle exec jekyll serve"를 실행한다.
10. 브라우저에 "localhost:4000"에 접속한다.
11. 기본 테마로 된 jekyll 사이트가 생성되었는지 확인한다.

### Post 변경하기
1. _posts 폴더에 "YYYY-MM-DD-TITLE.md" 형태의 새 문서를 생성한다.
2. Markdown 문법에 따라 내용을 작성한다.
3. "git add _posts/YYYY-MM-DD-TITLE.md"를 한다.
4. "git commit -m "커밋메세지""로 커밋한다.
5. "git push origin main"으로 원격저장소에 업로드한다.
6. 변경 내용을 확인한다.

### Theme 입히기
1. "Mr.Green"이라는 jekyll theme를 찾는다.
2. 해당 깃허브 사이트에 들억서 zip파일을 다운받는다.
3. 다운받은 파일을 원래 파일위에 덮어쓴다.
4. "git status"를 하여 추가받을 게 따로 있는지 확인한다.
5. "git add *"를 해서 변경 사항을 반영한다.
6. "git commit -m "커밋메세지""로 커밋한다.
7. "git push origin main"으로 원격저장소에 업로드한다.
8. 테마가 잘 적용되었는지 확인한다.

### 댓글 기능 추가하기
1. "https://disqus.com" 접속한다.
2. 회원가입 및 사이트 정보를 입력한다.
3. "_config.yml"파일에 필요한 내용을 추가한다.
   (나는 "posts.yml", "main.yml", "en.yml"파일을 수정했다.)
4. "git add *"를 해서 변경 사항을 반영한다.
5. "git commit -m "커밋메세지""로 커밋한다.
6. "git push origin main"으로 원격저장소에 업로드한다.
7. 댓글 기능이 추가되었는지, 잘 작동하는지 확인한다.

