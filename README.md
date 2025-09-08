# git - 간편 안내서
git을 시작하기 위한 간편 안내서. 어렵지 않아요 :)
저희 사무국에서 작성한 가이드 외에도 아래 가이드를 활용해보세요.

[추천 git 안내서 보러가기(클릭)](https://rogerdudler.github.io/git-guide/index.ko.html?utm_source=chatgpt.com)

## Git & GitHub 기초 사용법 가이드

### Git과 GitHub란?
- **Git**: 소스코드 버전 관리 시스템. 프로젝트의 변화 이력을 기록하고, 실수했을 때 되돌릴 수 있도록 하는 도구.[5]
- **GitHub**: Git 저장소를 인터넷에 저장·공유할 수 있는 웹 서비스. 협업이나 코드 공개, 포트폴리오 용도로 널리 사용됨.[1][5]

### 1. Git 설치 및 설정
- https://git-scm.com 에서 Git 다운로드 및 설치.[8][5]
- 최초 1회, 사용자 등록(이름/이메일):
  ```
  git config --global user.name "사용자이름"
  git config --global user.email "이메일주소"
  ```
  이 명령은 이후 커밋 기록에 표시됨.[4][5]

### 2. GitHub 계정 및 저장소 생성
- https://github.com 에 가입(무료).
- 로그인 후 'New' → 저장소 이름 입력 → 'Public(공개)' 또는 'Private(비공개)' 선택 후 생성.[2][3]
- (선택) README.md 파일 추가로 소개글 작성 가능.[3]

### 3. 프로젝트 폴더를 Git과 연결
1. 폴더를 만들고 이동:
   ```
   mkdir my-project
   cd my-project
   ```
2. Git 저장소 초기화:
   ```
   git init
   ```
   명령을 실행하면 Git이 폴더를 버전 관리 대상으로 인식.[4][5]

### 4. 버전 관리의 시작: 파일 추가, 커밋
- 변경사항 확인:  
  ```
  git status
  ```
- 새 파일 추가(스테이징):
  ```
  git add 파일명
  ```
- 커밋(저장):
  ```
  git commit -m "첫 커밋 메시지"
  ```
  커밋은 프로젝트의 순간 상태를 저장.[5][4]

### 5. GitHub와 연동 및 코드 업로드
- 원격 저장소 연결:
  ```
  git remote add origin https://github.com/내아이디/저장소이름.git
  git branch -M main
  ```
- 최초 업로드(Push):
  ```
  git push -u origin main
  ```
  이후부터는 변경/저장/업로드 순서로 반복.[6][4][5]

### 6. 협업과 버전관리에 자주 쓰는 명령어
- 기존 소스 최신화(가져오기):
  ```
  git pull
  ```
- 커밋 기록 보기:
  ```
  git log
  ```
- 새로운 변경 업로드:
  ```
  git add .
  git commit -m "변경사항 설명"
  git push
  ```


| 작업                 | 명령어                                      |
|----------------------|---------------------------------------------|
| Git 초기화           | git init                                    |
| 사용자 설정          | git config --global ...                      |
| 파일 추적            | git add 파일명                               |
| 커밋 생성            | git commit -m "메시지"                      |
| GitHub 연결          | git remote add origin URL                    |
| 브랜치 이름 변경     | git branch -m main                           |
| 코드 푸시            | git push origin main                         |
| 인증 저장            | git config --global credential.helper store   |
| 코드 가져오기        | git pull origin main                         |


  

***

