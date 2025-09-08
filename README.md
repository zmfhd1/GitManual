# git - 간편 안내서
git을 시작하기 위한 간편 안내서. 어렵지 않아요 :)

***

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

***

**참고**:  
- 파일/폴더 추가, 삭제, 브랜치 생성, 이슈 관리 등 더 많은 기능이 있으니 차근차근 익혀가면 좋습니다.[1][3][5]
- GitHub 웹 화면에서도 파일 추가 및 복사, README 수정이 가능합니다.[2][3]

[1](https://nbcamp.spartacodingclub.kr/blog/%EA%B0%9C%EB%B0%9C%EC%9E%90-%EC%B7%A8%EC%A4%80%EC%83%9D%EC%9D%84-%EC%9C%84%ED%95%9C-%EA%B9%83%ED%97%88%EB%B8%8C-%EA%B0%80%EC%9D%B4%EB%93%9C-git%EA%B3%BC-%EC%B0%A8%EC%9D%B4-%EC%82%AC%EC%9A%A9%EB%B2%95-%ED%94%84%EB%A1%9C%ED%95%84-%EA%BE%B8%EB%AF%B8%EA%B8%B0%EA%B9%8C%EC%A7%80-47204)
[2](https://maos.tistory.com/entry/%EA%B9%83%ED%97%88%EB%B8%8CGitHub-%EA%B0%80%EC%9E%85-%EB%B0%A9%EB%B2%95%EB%B6%80%ED%84%B0-%EC%A0%80%EC%9E%A5%EC%86%8C-%EC%83%9D%EC%84%B1%C2%B7%ED%8C%8C%EC%9D%BC-%EC%97%85%EB%A1%9C%EB%93%9C%EA%B9%8C%EC%A7%80-%EC%B4%88%EB%B3%B4%EC%9E%90%EB%A5%BC-%EC%9C%84%ED%95%9C-%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80-%EA%B0%80%EC%9D%B4%EB%93%9C-1)
[3](https://garoro77.tistory.com/entry/GitHub-%EC%82%AC%EC%9A%A9%EB%B2%95-%EC%99%84%EB%B2%BD-%EA%B0%80%EC%9D%B4%EB%93%9C-2025-%E2%80%93-%EC%B4%88%EB%B3%B4%EC%9E%90%EB%A5%BC-%EC%9C%84%ED%95%9C-%EA%B3%84%EC%A0%95-%EC%83%9D%EC%84%B1%EB%B6%80%ED%84%B0-%ED%98%91%EC%97%85%EA%B9%8C%EC%A7%80-%EB%8B%A8%EA%B3%84%EB%B3%84-%EC%84%A4%EB%AA%85)
[4](https://www.jiniai.biz/2025/05/08/git-github-%EA%B8%B0%EC%B4%88-%EC%82%AC%EC%9A%A9%EB%B2%95-%EC%99%84%EC%A0%84-%EC%A0%95%EB%B3%B5-%EB%8B%A8%EA%B3%84%EB%B3%84-%EC%98%88%EC%A0%9C%EC%99%80-%ED%95%A8%EA%BB%98-%EB%B0%B0%EC%9A%B0/)
[5](https://commutemochabread.tistory.com/44)
[6](https://commutemochabread.tistory.com/29)
[7](https://wooniblo.com/entry/2025-%EC%B5%9C%EC%8B%A0-%EC%B4%88%EB%B3%B4%EC%9E%90%EB%A5%BC-%EC%9C%84%ED%95%9C-Git-GitHub-%EC%82%AC%EC%9A%A9%EB%B2%95-%EB%B2%84%EC%A0%84-%EA%B4%80%EB%A6%AC-%ED%95%84%EC%88%98-%EC%8A%A4%ED%82%AC)
[8](https://aspdotnet.tistory.com/3415)
[9](https://garoro77.tistory.com/entry/%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4-%EA%B8%B0%EC%97%AC-%EB%B0%A9%EB%B2%95-%EC%99%84%EB%B2%BD-%EA%B0%80%EC%9D%B4%EB%93%9C-%E2%80%93-%EC%B4%88%EB%B3%B4-%EA%B0%9C%EB%B0%9C%EC%9E%90%EB%8F%84-%EC%8B%9C%EC%9E%91%ED%95%A0-%EC%88%98-%EC%9E%88%EB%8A%94-2025%EB%85%84-%EC%8B%A4%EC%A0%84-%ED%8C%81)
