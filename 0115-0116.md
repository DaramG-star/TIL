# 0115 ~ 0116 TIL

## 1. Markdown 사용법 익히기
굵게 만들기 : 양옆으로 * 2개.

**굵어져라 굵어져라**

기울이기 : 양옆으로 * 1개.

*기울이기 기울이기*

취소선 : 양옆으로 ~ 2개.

~~취소 취소~~

수평선 : - 3개이상 적기

---

- 순서가 없는 리스트
    - 어디까지
        - 여기까지

1. 순서가 있는 리스트
    
    2. 2번순서
            
            3. 3번순서

```
T = int(input())
```
프로그래밍 스타일에 맞춰 텍스트 스타일 변환

[나의 github](https://github.com/DaramG-star)

![이미지](https://picsum.photos/200/300)

## 2. GUI와 CUI
```
GUI : 그래픽을 통해 사용자와 컴퓨터가 상호 작용하는 방식
```
```
CLI : 명령어를 통해 사용자와 컴퓨터가 상호 작용하는 방식  
```
CLI는 키보드만으로 모든 작업을 수행할 수 있고, 메모리와 CPU 사용량이 적어 저사양 시스템에서도 효율적으로 동작.

특정 프로그램이나 시스템의 세부 설정을 보다 정밀하게 제어할 수 있음.

CLI 명령어는 대부분의 Unix 운영체제 기반 시스템에서 동일하게 동작하여 여러 환경에서 적용할 수 있음.

## 3. GIT과 친해지기
### 기초문법
- touch : 파일 생성

- mkdir : 새 디렉토리 생성

- ls : 현재 작업중인 디렉토리 내부의 폴더/파일 목록 출력

- cd : 현재 작업중인 디렉토리를 변경

- start : 폴더/파일을 열기

- rm : 파일 삭제

```
GIT 이란 ?
```
분산 버전 관리 시스템.

변화를 기록하고 추적하는 것을 버전관리라고 한다.

```
Working Directory란?
```
실제 작업중인 파일들이 위치하는 영역

```
Staging Area란?
```
Working Directory에서 변경된 파일 중, 다음 버전에 포함시킬 파일들을 선택적으로 추가하거나 제외할 수 있는 중간 준비 영역

```
Repository란?
```
버전 이력과 파일들이 영구적으로 저장되는 영역

```
commit이란?
```
변경된 파일들을 저장하는 행위이며, 마치 사진을 찍듯이 기록한다 하여 'snapshot'이라고도 함.

---

### git의 동작

```
git init
```
로컬 저장소 설정(초기화)

-> git의 버전 관리를 시작할 디렉토리에서 진행

```
git add
```
변경사항이 있는 파일을 staging area에 추가

```
git commit
```
staging area에 있는 파일들을 저장소에 기록

-> 해당 시점의 버전을 생성하고 변경 이력을 남기는 것.

! 일단 해본 결과 vs code에서는 그냥 돋보기 밑에 있는 버튼만 누르면 commit이랑 add 명령어 자동으로 됨!

```
git config --global user.email "메일주소"

git config --global user.name "유저네임"
```
commit 작성자 정보 설정 방법

```
git status
```
현재 로컬 저장소의 파일 상태 보기

```
git log, git log--oneline
```
commit 목록 보기
```
git config --global -l
```
git global 설정 정보 보기

```
git commit --amend
```
commit 메시지 수정

수정 후, :wq 적어서 저장 후 빠져나오면 됨.

---

### 원격저장소


코드와 버전 관리 이력을 온라인 상의 특정 위치에 저장하여 여러 개발자가 협업하고 코드를 공유할 수 있는 저장 공간

```
git remote add origin (url)
```
로컬 저장소에 원격 저장소 추가

```
git push origin master
```
원격 저장소에 commit 목록을 업로드

```
git pull origin master
```
원격 저장소의 변경사항만을 받아옴

```
git clone (url)
```
원격 저장소 전체 복제

```
gitignore
```
Git에서 특정 파일이나 디렉토리를 추적하지 않도록 설정하는 데 사용되는 텍스트 파일


