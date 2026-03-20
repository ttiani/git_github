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
   1. url = https://본인계정:토큰@github.com/본인레파지토리명.git

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

# 2.github
원격 저장소

