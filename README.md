### git을 시작하는 방법을 정리 

## git 계정및 아이디 정보 설정
git config --global user.email "test-user@gmail.com"
git config -- user.name "test-user"

## 1. repository를 만들고 아무것도 없는상태에서 push 하기
```
echo "# test" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/chuls-hops/test.git
git push -u origin main
```

## 2. 이미 만들어진 상태에서 내려 받은후 변경하고 push 하기 
```
mkdir test
cd test
git clone remote add origin https://github.com/chuls-hops/test.git . 
- . 을 찍어야 현재디렉토리 내려옴, 안찍으면 현재디렉토리 아래에 test폴더 밑에 데이터가 내려옴
git remote add origin https://github.com/chuls-hops/test.git
git branch -M main
git add README.md
git commit -m "second commit"
git push -u origin main
```




## 최초레포 만들면 나오는 메시지 


### Quick setup — if you’ve done this kind of thing before
### Set up in Desktop
### or
### HTTPSSSH
### Get started by creating a new file or uploading an existing file. We recommend every repository include a README, LICENSE, and .gitignore.
### … or create a new repository on the command line
```
echo "# test" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/chuls-hops/test.git
git push -u origin main
```
### …or push an existing repository from the command line
```
git remote add origin https://github.com/chuls-hops/test.git
git branch -M main
git push -u origin main
```
###  …or import code from another repository
You can initialize this repository with code from a Subversion, Mercurial, or TFS project.
Import code
