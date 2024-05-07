# ⚙️ ️작업 세팅!
### 1. 프로젝트 만들기
- 원하는 directory 안에 Capstone 폴더 생성
- IntellJ 켜서 열기 누르고 방금 만든 Capstone 폴더 선택
- Capstone 안에 .idea 폴더 삭제(계속 생길건데 처음 한번만 삭제)

-----

### 2. 프로젝트 clone 하기
- IntellJ 왼쪽 하단 터미널창 열고 git Bash 열기


![](images/git1.png)
- 터미널 창에 아래 코드 입력 (Capstone_back 프로젝트 clone)
#### ```git clone https://github.com/Hichanmin/Capstone-back.git```
- 터미널 창에 아래 코드 입력 (Capstone_front 프로젝트 clone)
#### ```git clone https://github.com/tgyeom/Capston_front.git```
- 터미널 창에 아래 코드 입력(Git_Capstone 프로젝트 clone)
#### ```git clone https://github.com/Hichanmin/Git_Capstone```

-----

### 3. Capstone_back 프로젝트 세팅
- IntellJ 오른쪽 상단 파일 -> 열기 -> Capstone_back 폴더 선택 -> 이 창에서 열기
- clone 해오면 자동으로 clone 받아온 repository 에 remote 됩니다.

>IntellJ 에서 파일 열기로 Capstone_back 을 하면 우리 백엔드 repository 연결되고
>
>IntellJ 에서 파일 열기로 Capstone_front 를 하면 태겸이네 프론트 repository 연결되고
> 
>IntellJ 에서 파일 열기로 Git_Capstone 을 하면 깃 repository 연결된게 정상
- 터미널 창에 아래 코드 입력 (현재 연결된 git repository 확인)
#### ```git remote -v```
- 터미널 창에 아래 코드 입력 (위에 실행했을 때 연결된 레포가 없을 때만)
#### ```git remote add origin https://github.com/Hichanmin/Capstone-back.git```

-----
# 🔧 작업 시작!
### 1. branch 만들고 checkout 하기
- 터미널 창에 아래 코드 입력
#### ```git branch 이름_dev```
#### ```git checkout Chanmin_dev```
- IntellJ 왼쪽 상단 보고 checkout 됐는지 확인


  ![](images/git2.png)

[잘못 만들었을 때 삭제하고 싶으면 다시 main branch 로 checkout 후에 아래 코드 입력]
#### ```git branch -d Chanmin_dev```
### 2. 코드 개발 시작

----

# 🎢 작업 올리기!
### 1. 깃 add, commit, push 하기
#### 밑에 하면서 global 어쩌구 나오면 git global config add user.email 하고 user.name 이거 안돼서 그럴걸
- 터미널 창에 아래 코드 입력(add)
#### ```git add .```
- 터미널 창에 아래 코드 입력(commit)
#### ```git commit -m "xx기능 구현"```
- 터미널 창에 아래 코드 입력(push)
#### ```git push origin Chanmin_dev```

### 2. pull request
![](images/git3.png)
![](images/git4.png)
![](images/git5.png)
![](images/git6.png)
![](images/git7.png)

----

# 📋작업 마무리!
### 1. main branch 로 checkout 후에 Chanmin_dev branch 삭제
#### ```git checkout main```
#### ```git branch -d Chanmin_dev```
! 오류가 난다면 거의 Chanmin_dev branch가 수정된 사항이 있어서 그럴 확률이 매우 높음
[클릭](#-작업-올리기) 이거 1번만 다시하면 아마 될겁니다.
### 2. merge(병합)된 main branch(원격) 를 main branch(로컬) 로 pull 하기
#### ```git pull origin main```