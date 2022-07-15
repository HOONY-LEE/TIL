## Git이란?

- 분산 버전 관리 프로그램
- 코드의 히스토리(버전)을 관리하는 도구
- 개발되어온 과정 파악 가능
- 이전 버전과 변경 사항을 비교 분석 가능(git diff)

## Git이 코드 버전을 관리하는 방식

1. 파일에 날짜와 시간을 적는다.
2. 변경 사항만 기록한다.
3. 맨 나중 파일과 이전 변경사항만 남긴다.

### 1. 중앙 집중식 버전 관리

ex) 금융서버

### 2. 분산 버전 관리

ex) 블록체인, Git

```
                       서버 컴퓨터(클라우드)

                    /                               \\

           컴퓨터 A                               컴퓨터B
```

Git 기반의 저장소 서비스를 제공하는 서버 = { GitHub , GitLab 등등 }

## GUI란?

- Graphic User Interface
- 그래픽을 통해 사용자와 컴퓨터가 상호 작용하는 방식
- ex) 윈도우, 바탕화면 등
- CLI에서만 할 수 있는 작업이 있음

## CLI란?

- Command Line Interface
- ex) 명령 프롬프트, POWERSHELL, 터미널,  GITBASH 등
- 명령어를 통해 사용자와 컴퓨터가 상호작용하는 방식
- GUI에 비해서 컴퓨터의 리소스 절약이 많이 됨
- 수 많은 서버/ 개발 시스템이 CLI를 통한 조작 환경을 제공

## 기본적인 명령어

- touch :  새로운 파일 생성
- mkdir : 새로운 디렉터리 생성
- ls : 현재 작업중인 디렉터리의 폴도/ 파일 목록을 보여줌
- cd : 현재 작업 중인 디렉토리를 변경(이동)
- cd ../ : 현재 위치에서 상위 폴더로 이동
- start/ open : 폴더/파일을 여는 명령어(window/ Mac)
- rm : 파일을 삭제
- rm -r : 디렉터리 삭제

## 상대경로 vs 절대경로

### 절대경로

- 루트 디렉토리부터 목적 지점까지 거치는 모든 경로를 전부 작성한것
- 윈도우 바탕화면의 절대경로  C:/Users/ssafy/Desktop

### 상대경로

- 현재 작업하고 있는 디렉토리를 기준으로 계산된 상대적인 위치를 작성한 것
- 윈도우 바탕화면의 상대 경로 ssafy/Desktop
- ./ : 현재 폴더
- ../ : 현재 폴더의 부모 폴더

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d6a30d1c-d456-483b-b645-00fd98f69dc3/Untitled.png)

~ 는 자주 사용하는 경로를 축약한 형태로

C:\Users\multicampus 유저의 홈 디렉터리를 뜻함

------

- 개발자들이 Mac OS를 선호하는 이유

Linux / Unix → Mac OS

최근 MS에서도 Powershell을 통해 개발자들이 Linux기반 명령어를 사용할 수 있게함





- [READ.md](http://READ.md) 생성하기
- 이 파일을 버전 관리하여 Git 사용하기
- → 특정 버전으로 남긴다 = “커밋(commit)한다”



## 커밋(commit) 은 3가지 영역을 바탕으로 동작

1. Working Directory
   - 내가 작업하고 있는 실제 디렉토리
2. Staging Area
   - 커밋으로 남기고 싶은 특정 버전으로 관리하고 싶은 파일이 잠시 있는 곳
3. Repository
   - 커밋(commit)들이 저장되는 곳

## Repository(저장소)

- git init 명령어로 로컬 저장소를 생성
- .git(숨김) 디렉토리에 버전 관리에 필요한 모든 것이 들어있음

# STARTCAMP 2일차

## untracked

최초 아직 git이 변경사항을 추적하지 않은 상태

## 1. git add

워킹디렉토리에 있는 untracked  파일을  staging area로 올라감

untracked → staged

## 2. git commit :

staging area에 올라간 변경된 사항을 repository에 저장

committed

untracked → modified

## 3. git status

- 현재 git으로 관리되고 있는 파일들의 상태를 알 수 있음

git init

git add .

git commit -m “[수정했음]”

git log

git status

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c78b62b7-a620-4789-b497-10585662c569/Untitled.png)

오늘 해볼 과제

ctrl + c 잘 못입력한 콘솔창 다시 초기화

git log : git commit history 보기

git diff :  두  commit 간 차이 보기

desktop 하위에 edu_git 디렉터리을 만든다

## 왜 굳이 중간에 Staging Area에 남길까?

여러가지 작업 중에서 완료된 작업만 commit에 남기고 변경만 된 파일은 staging area에 남겨놓는다.

## remote repository에 연결하기

- git remote add origin {remote_repo}
- git push origin(어디로) master(커밋이 쌓인 마스터 브랜치)
- 

```python
단축키 모음
( Ctrl + K ) + F     VS코드에서 폴더 닫기
Ctrl + Shift + ` vs코드에서 터미널 열기
code
```

## TIL(Today I Learned)

- 매일 내가 배운 것을 마크다운으로 정리해서 문서화하는 것
- 신입 개발자에게 요구되는 가장 큰 능력
- Github 관리의 가장 큰 첫 걸음