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