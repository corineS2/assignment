## 깃 전체 도움말 보기
```
$git help
```

## 버전 정보 확인
```
$git version
```

## 사용자 기본 설정
```
$git config --global user.name
```
```
$git config --global user.email
```

### 맥과 윈도간의 자동 변환
```
$git config --global core.autocrlf true
```

### 뉴라인 경고 발생 없애기
```
$git config --global core.safecrlf false
```

### 깃 명령어 별칭 설정
```
$git config --global alias.별칭 '별칭을 주려는 명령어'
```

### 기본 브랜치를 main으로 설정
```
$git config init.default Branch main
```

## 전역 환경설정 확인
```
$git config --global --list
```

### 전역설정파일 편집
```
$git config --global -e
```

### 전역 설정값 확인
```
$git config --global --get
```

## 지역 환경 설정 확인(현재 설정 확인)
```
$git config --list
```

### 지역 설정 파일 편집
```
$git config -e
```

### 지역 설정값 확인
```
$git config --get
```

## 깃 저장소(폴더) 생성
```
$git init
```

## 상태보기
```
$git status
```

## 커밋 내역 확인
```
$git log
```

## 가장 최근 커밋 확인
```
$git show
```

## 스테이지에 저장
```
$git add
```

## 메모와 함께 커밋
```
$git commit -m '메모'
```

### add와 commit을 한번에 수행
```
$git commit -am
```

## 원격저장소에서 로컬 저장소로 가져오기
```
$git pull
```
### 원격저장소에서 로컬 저장소로 가져오기
차이점 : 로컬 저장소와 원격 저장소의 변경 사항이 다를 때 이를 비교 대조하고 git merge 명령어와 함께 최신 데이터를 반영하거나 충돌 문제 등을 해결
```
$git fetch <remote>
```

## 로컬저장소에서 원격 저장소로 내보내기
```
$git push
```

## 원격저장소에서 로컬저장소로 복제하기(동일 폴더 생성)
```
$git clone 주소
```

## 원격 저장소 별칭 이름 조회
```
$git remote
```

### 원격 저장소 별칭 추가
```
$git remote add 별칭 주소
```

### 원격저장소명을 지정한 별칭으로 변경
```
$git clone 주소 -o 별칭
```

## 브랜치 이동
```
$git switch
```
```
$git checkout
```

### 브랜치 생성, 생성한 브랜치로 이동
```
$git switch -c
```
```
$git checkout -b
```

## 시간 여행하기
```
$git checkout HEAD~(HEAD~~/HEAD/main)
```

## 브랜치 생성
```
$git branch 브랜치명
```

### 브랜치 목록 보기
```
$git branch
```

## SA와 WD 비교
```
$git diff
```

### HEAD와 WD 비교
```
$git diff head
```

### HEAD~(이전 커밋 내역)와 WD 비교
```
$git diff head~
```

## HEAD와 SA 비교
```
$git diff --staged
```
```
$git diff --cached
```

### HEAD~(이전 커밋 내역)와 SA 비교
```
$git diff --cached head~
```

## WD에는 남겨두고 SA만 파일 삭제
```
$git rm --cached
```

## WD의 수정내역 취소
```
$git restore
```

### SA를 이전 상태로 변경
```
$git restore --staged
```

## 현재브랜치에서 대상브랜치를 병합(= fast forward merge)
서로 다른 상태를 병합하는 것이 아닌, main을 my-branch 위치로 이동
```
$git merge 브랜치명
```

### non fast forward로 merge(= 3-way merge)
하나의 브랜치와 다른 브랜치의 모든 변경 이력 합치기
```
$git merge --no-ff 브랜치명
```

## 한 브랜치에서 다른 브랜치를 이어붙이기 병합
히스토리가 선형으로 단순
```
$ git rebase 브랜치명
```


