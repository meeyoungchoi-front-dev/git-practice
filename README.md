# 정리

## 하나의 버전이 만들어지는 과정

### 작업 디렉터리 내에서 변경 사항 생성

### 스테이지로 add

### 저장소로 commit (커밋메시지: 버전에 대한 설명)

![alt text](image.png)

## 커밋에 대한 태그
![alt text](image-1.png)
![alt text](image-2.png)


# 이미 만들어진 버전을 되돌리는 두 가지 방법

## revert : 버전을 되돌린 새로운 버전을 만든다
- 기존에 만들어 뒀던 버전은 유지가 된체 버전을 되돌린 새로운 버전을 만드는것
![alt text](image-3.png)
![alt text](image-4.png)

## reset : 버전을 완전히 되돌린다 (만들어뒀던 작업 내역들이 사라지게 된다)
1. soft : 저장소로 커밋하기 만 되돌리는 단계
![alt text](image-5.png)
![alt text](image-6.png)
![alt text](image-7.png)
- 커밋을 했다라는 사실만을 되돌린 것이다
-  따라서 파일상태 변경사항에는 남아있게 된다

2. mixed : 스테이지로 추가했다는 사실까지 되될리는 단계
3. hard : 작업 디렉터리에서 변경 사항을 생성했다는 사실까지 되돌리는 단계

# 작업을 임시저장하는 방법 (stash)
![alt text](image-8.png)
![alt text](image-9.png)
![alt text](image-10.png)

# 브랜치로 나누어 관리하기
## 브랜치란 : 버전의 흐름, 버전
![alt text](image-12.png)
![alt text](image-13.png)
![alt text](image-14.png)
![alt text](image-15.png)
## 브랜치의 이름: 최초의 브랜치, master 브랜치
- 가장 기존적인 브랜치이다
- 깃허브에서는 main 브랜치라고 부른다

## 브랜치 이름
- 예) feature/menu 브랜치 (메뉴 기능 추가를 위한 브랜치)
- 예) hotfix/login 브랜치 (로그인 기능을 급하게 수정하기 위한 브랜치)
- 예) release/2.3.0 브랜치 (2.3.0 버전 릴리스를 위한 브랜치)

## 특정 브랜치에서 작업하기 : HEAD와 체크아웃
1. Head
+ 현재 작업중인 브랜치의 최신 커밋을 가리킨다
+ 내가 지금 어디에서 작업중인지를 가리킨다

2. 체크아웃
+ 특정 브랜치에서 작업할 수 있도록 작업 환경을 바꾸는것
+ HEAD의 위치를 특정 브랜치의 최신 커밋으로 옮기는 것

## 브랜치를 합친다 merge
![alt text](image-16.png)
![alt text](image-17.png)
![alt text](image-18.png)
![alt text](image-19.png)
![alt text](image-20.png)
![alt text](image-21.png)
![alt text](image-22.png)

## 브랜치 충돌 
![alt text](image-23.png)
![alt text](image-24.png)
![alt text](image-25.png)
![alt text](image-26.png)
## 위 4번째 그림에 대한 설명
<<<<<<< HEAD
a-1.txt 파일의 같은 내용을 다르게 수정 <-------------------  현재 브랜치 (master) 브랜치 내용
=======
foo  <-------- foo 브랜치 내용
>>>>>>> foo

## master 브랜치의 내용으로 병합하여 충돌 해결
![alt text](image-27.png)
![alt text](image-28.png)

## a-1.txt 파일을 열어보면 master 브랜치의 내용이 반영이 되어 있다
![alt text](image-29.png)

## foo branch와 master branch를 병합했을때 나오는 새로운 branch
![alt text](image-30.png)

# rebase branch
![alt text](image-31.png)
![alt text](image-32.png)
![alt text](image-33.png)
![alt text](image-34.png)
![alt text](image-35.png)