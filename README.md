# Git-Start

## 간단한 리눅스 명령어

### cd

- change directory의 약자.
- 디렉터리를 변경하는 명령어

```bash
cd test    # test 디렉터리로 이동
cd .       # 현재 디렉터리로 이동
cd ..      # 부모 디렉터리로 이동
cd ~       # home 디렉터리로 이동
```

### mkdir

- make directory의 약자
- 디렉터리를 생성하는 명령어

```bash
mkdir test_dir      # test_dir 디렉터리 생성 - 새폴더
```

### ls

- list의 약자
- 파일, 디렉터리 목록을 보여주는 명령어

```bash
ls                 # 현재 디렉터리에 있는 파일과 디렉터리 목록을 보여줌
ls ./test_dir      # test_dir의 파일, 디렉터리 목록을 보여준다.
ls -al             # 현재 디렉터리에 있는 파일, 디렉터리 목록을 자세히 보여준다.(옵션은 -를 붙여서 씀, -a와 -l이 더해져 있음)
```

### cat

- concatenate의 약자(연결하다)
- 파일 내용을 확인할 때 사용하는 명령어

```bash
cat text.java               # test.java의 내용을 보여준다.
cat test.java | more        # test.java의 파일을 보여주되, 내용을 전부 보여주지 않고 더 보기(more) 상태로 보여줌.
```

> `<br>`은 엔터, `<hr>` 선 긋기

<br><hr>

## Git 명령어

- Git은 버전 관리 소프트웨어, `VCS(Version Control System)` 중 가장 보편적인 소프트웨어.

### git init

- git으로 버전 관리할 폴더를 저장한다.
- `.git` 이라는 폴더가 생성이 됨.

```bash
git init
```

### git add

- 현재 추적 중이지 않은 파일을 추적 상태로 바꾸는 용도로 사용한다. (untracked --> staging)
- 변경된 파일을 staging에 올릴 때도 사용한다. (modified --> staging)

```bash
git add test.java
```

### git commit

- 현재 staging 위에 올라가 있는 모든 파일들을 가지고 하나의 버전을 생성한다.
- 하나의 버전이 생성되면 그 버전은 hash 값으로 관리된다.

```bash
git commit -m "커밋 메시지"     #메시지를 남김
```

### git log

- 현재 git이 관리하고 있는 폴더의 모든 커밋을 보여준다.

```bash
git log
git log --oneline
```

### git checkout

- 다른 브랜치 또는 다른 commit으로 이동하고 싶을 때 사용하는 명령어

```bash
git checkout 8d2bead        # 특정 커밋으로 이동
git checkout master         # master 브랜치로 이동
```

### git push

- github에 새로 추가된 커밋들을 업로드하는 명령어.

```bash
git push origin master       # git push [alias] [branch]
```

### git pull

- github에 업로드 된 커밋들을 내 로컬 브랜치로 가져오는 명령어.

```bash
git pull origin master      # git pull [alias] [branch]
```

### git status

- git의 현재 상태를 보여주는 명령어

```bash
git status
```

### git merge

- 서로 다른 브랜치에 있는 내용을 병합할 때 사용하는 명령어
- develop --> master

```bash
git checkout master       # 병합하고자 하는 브랜치로 이동
git merge develop         # develop에 있는 내용을 master로 병합한다.
```

</br><hr>

## 항목

- 항목1
- 항목2
  - 세부항목1
  - 세부항목2
    - 세세부항목1

### 체크박스

- [ ] 체크박스1
- [x] 체크박스2

> 인용문구 작성 가능

#### 텍스트

데이터를 강조하고 싶을 땐 **강조** 사용합니다.

데이터 강조하고 싶을 땐 **_강조_** 를 사용합니다.

취소선은 ~~취소~~ 입니다.

##### 코드삽입

```java

public int add(int x, int y){
    return x + y;
}
// 주석입니다.
```

```sql

SELECT *
FROM users
WHERE users.id = 1;
```

##### 이미지, 링크 삽입

![이미지](./capture.PNG)

[네이버링크](https://www.naver.com)
