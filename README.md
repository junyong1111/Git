# Git

## Git의 배경
Unix라는 대형컴퓨터 운영체제를 리눅스 토발즈가 개인용 컴퓨터 OS로 발전시키며 이것이 리눅스이다.
* GNU: 공개 소프트웨어 프로젝트  
어떤 소프트웨어A를 누구에게나 공개 단, 공개된 소프트웨어 정보를 받았을 시 GPL 라이센스를 따야함 
* GPL (General Public License): A소프트웨어로 B소프트웨어를 만들 시 B소프트웨어는 무조건 공개되어야 한다.  

리눅스를 수 많은 개발자들이 발전시켜가는 과정에서 협업이 필요한데 각자가 개발한 파일을 합쳐야 하는 문제점등이 존재하여 이를 해결하기 위해서 Bitkeeper라는 분산 버전 관리 시스템을 상용화시킴 (Distribution Version Contrl System)사용자가 많아짐에 따라 Bitkkeper가 유료화서비스를 시작하려 하자 리눅스 토발즈가 만든 버전 관리 시스템이 바로 Git이다

## Github

* 모든 개발자들의 놀이터
* 개발자들의 코드가 저장되는 클라우드는 저장소 Git과는 다르기 때문에 GPL라이센스를 따르지않는다
* 마이크로소프트가 Github를 인수
* Public : 나의 모든 소스를 공개
* Private : 나의 모든 소스를 비공개
* MIT라이센스 : 공개된 소스코드로 개발을 해도 공개 의무가 없는 MIT라인센스를 따른다. 

## 실습 

### 저장소 생성 및 깃허브 연동

1. 저장소 생성
    
    ```bash
    echo "Hello World" > index.html
    위 명령어로 파일 하나 생성
    
    git init .
    위 명령어로 시작
    
    ls -a
    위 명령어로 숨겨진 폴더 확인
    ```
    
    디렉토리 구조
    
    GIT
    
    - index.html
    
    → git.init 명령어를 통해서 숨겨진 .git 폴더가 생성이 되며 깃 관리 이 숨겨진 폴더를 삭제하면 본래 기본 폴더가 되며 복사할 때는 숨겨진 폴더도 같이 해줘야 한다.
    
2. 깃 저장소 종류

Git은 분산형 관리 시스템

- 로컬 저장소
    - 자기 컴퓨터에 있는 저장소
- 원격 저장소
    - 자기 컴퓨터가 아닌 외부 저장소
    - 보다 협업을 쉽게 하기 위해서 공통된 서버 개념에 저장소라고 생각
    - Github을 이용하여 원격 서버 저장소를 이용가능
1. Github에서 저장소 하나 생성
    - 생성한 저장소를 로컬 저장소에 등록
    
    ```bash
    git remote add origin "생성한 저장소 주소"
    위 명령어를 통해 로컬 저장소에 원격 저장소를 등록
    
    git remote -v 
    등록된 원격 저장소 확인
    ```
    

### 커밋 및 전송하기


=======

## Info_Git

기본적인 Git에대한 공부와함게  github와 gitblog만드는 방법 Markdown문법을 설명
git config --list (현재 폴더내에서 git정보확인)
git config user.name "이름"
git config user.email "gitgub 주소"

git 시작시 git pull로 로컬저장소로 내용들을 가져온다음 시작

