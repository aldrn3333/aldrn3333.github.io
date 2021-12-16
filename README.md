## Make Git Blog!! 

## How to Make Git Blog?  

- Repository 생성   
- Git clone을 이용해 로컬 저장소 생성
- 실습 따라하며 로컬과 원격 저장소 연동 확인
- Jekyll 설치
- Theme 적용 
- Theme fork
- 파일 내용 변경
- navigation bar 수정
- 사이트 내 배경이미지 변경 및 favicon 추가
- Post 작성
- 댓글 기능 추가(Disqus)

### 1. Repository 생성  
Git 설치 이후, Github 계정에 aldrn3333.github.io 이름의 Repository를 생성했습니다.  

### 2. Local-Remote Repository 연동  
Git CMD에서 `git clone aldrn333.github.io`를 통해 Remote Repository의 주소를 복사하여 Local-Remote Repository를 연동했습니다.

### 3. 예시 문서 작성 후 원격 저장소 반영 시도
VS code를 이용해 예시 파일(index.html) 작성한 후,   
Git CMD에서 git add, git commit -m "", git push를 이용해 원격 저장소에 연동

### 4. Jekyll 설치  
Window를 이용해 진행했기에, Jekyll을 설치하기 전에 https://rubyinstaller.org/downloads/ 다음과 같은 사이트 접속하여 Ruby와 Devkit을 설치했습니다.  
이후 `gem install jekyll bundler` 명령어를 이용해 Jekyll을 설치했습니다.   
( Jekyll이 정상적으로 설치되어 있는지 확인하기 위해 `jekyll -v` 명령어를 이용했습니다. )  
이후 현재 디렉토리(Git Blog 디렉토리)에 `jekyll new . -- force` 명령어를 통해 Jekyll 설치를 완료했습니다.    
`(bundle exec) jekyll serve`명령어로 Jekyll를 실행하여 기본 테마로 된 Jekyll 사이트가 생성됨을 확인할 수 있었습니다.   

### 5. Theme 적용 ( 처음부터 다시 시작.. ) 
기본테마가 너무 밋밋했기에 새로운 태마를 아래의 두가지 사이트를 이용해 찾아보았습니다.    
http://jekyllthemes.org/, https://jekyllthemes.io/free      
원하는 테마를 찾아 zip 파일로 다운을 하고 로컬 저장소에 복사 및 붙여넣기를 했지만 오류가 발생했습니다

### 6. Theme fork
기존의 방법으로 테마를 적용했을 때 오류가 발생했으므로 강의에 나와 있는 내용을 토대로 fork를 이용해 원하는 테마를 가져와서 이름을 aldrn3333.github.io로 바꾸고 다시 git clone aldrn3333.github.io를 통해 로컬 저장소를 만들었습니다.

### 7. 파일 내용 변경 
모든 파일을 하나하나 들어가보며 대부분의 블로그 속성을 관리하는 _config.yml부터 시작해서 index.html, _includes 폴더 내의 header.html 등 다양한 파일의 내용들을 제 블로그의 컨셉에 맞게 수정했습니다.

### 8. navigation bar 수정
Home과 Github, instagram의 nav를 생성하여 Home을 누르게 되면 index.html에 연결되어 있어 홈페이지의 초기화면으로 돌아가도록 설정했으며, Github를 누르게 되면 새 창이 띄워지며 실제 제 Github가 띄워지도록 했고 instagram을 누르게 되면 저의 인스타그램으로 들어 가도록 했습니다.

### 9. 사이트 내 배경이미지 변경 및 favicon 추가
제 블로그의 컨셉에 맞게 수정하기 위해 assets/img 폴더 내애 기존에 있었던 이미지들을 삭제하고 저의 이미지로 대체하여 사이트의 배경사진을 변경했습니다.    
  

### 10. Post 작성
_posts 폴더에 특강에서 다뤄줬던 내용을 주제에 관해 post를 작성했습니다.YYYY-MM-DD-TITLE.md 형태로 새로운 문서를 생성하였으며 Markdown 형식으로 내용을 작성했습니다.   

### 11. 댓글 기능 추가(Disqus) 
댓글 기능을 추가하기 위해 Disqus에 가입 및 세팅을 진행했습니다.   
이후 _config.yml에 key-vale를 추가했으며, disqus 홈페이지에서 Universal Code를 복사한 후, _layouts/post.html에 복사한 코드를 붙여넣고 강의자료를 참고해 일부 코드를 추가했습니다.  
실제 post의 댓글 기능을 추가하기 위해 각 post마다 comments: True 설정을 추가했습니다.  

