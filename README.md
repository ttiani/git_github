# 1.git 
로컬 저장소

## 1.1 로컬 저장소 초기화
```bash
git init
```
<br>

## 1.2 로컬 저장소에 원격 저장소 지정
```bash
git remote add origin 원격 저장소 주소.git
```
<br>

## 1.3 branch 통합
```bash
git branch -M 브랜치명
``` 
<br>

## 1.4 토큰 등록
1. `.git/config` 파일 열기
2. [remote "origin"] 항목의 url 값에 토큰과 계정을 추가
   
   i. url = https://본인계정:토큰@github.com/깃허브레포지터리주소.git

<br>

## 1.5 작업 목록에 추가
```bash
git add 작업 파일명
git add .(현재파일의 모든 것)
```

<br>

## 1.6 커밋
```bash
git commit -m "커밋 메시지"
```

<br>

## 1.7 깃 허브에 배포
```bash
git push -u origin main
```

<br>

# 2. git 작업

## 2.1 github 복제
i. 레포지토리 모든 내용 복제
```bash
git clone 레포지토리이름
```
정상 완료 : 레포지토리명으로 지정한 로컬 저장소에 디렉토리 생성

<br>

ii. 특정 브랜치만 복제할 경우, 
git clone -b 브랜치명 --single-branch 레포지토리주소.git

<br>

iii. main, dev, design 브랜치가 존재하는 경우
```bash
git clone 레포지토리이름
cd git_github(clone폴더)

git checkout dev
git checkout main
git checkout design

git branch -M dev(브랜치 생성)
```

## 2.2 git fork
i. 본인 계정 log in

ii. fork 실행 git 주소로 이동

iii. 오른쪽 중상단 fork 버튼 클릭

iv. 현재의 repository와 구분된 별도 repository 생성 후 실행

v. fork 한 주소의 토큰이 없음 : 수정 불가

vi. 수정을 원할 경우, git pull을 통해 로컬 저장소에 저장후 가능

<br>



# 3. git pull
## 3.1 pull all
```bash
git init
git remote add origin 레포지토리주소.git
git pull 레포지토리주소.git
```

<br>

## 3.2 특정 브랜치만 pull

```bash
git branch -M 브랜치명
git pull origin 브랜치명
```