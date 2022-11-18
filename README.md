# 초보 개발자의 개발 일지
------------

* #### name : 이예찬
* #### email : 11chan11@naver.com

-------

[![네이버클라우드](./202209290853594643582.png "ncloud")](https://www.navercloudcorp.com/) AIaaS 개발자 과정 1기<br>

---
3차 실습
vagrant설치&vm생성&리눅스 설치&git설치&nano설치&git초기설정
1. 홈폴더에 vm-projects폴더 생성
mkdir vm-projects
2. vm-projects 폴더 접속
cd vm-projects
3. centos 폴더 생성
mkdir centos
4. centos 폴더 접속
cd centos
5. centos 이미지 파일 다운로드
vagrant init "centos/7"
6. vagrantfile에서 config.vm.hostname = "myhost5.bitcamp" 입력
7. vagrant 설정 파일 다운로드 및 실행
vagrant up 
8. vm에서 ssh로 접속
vagrant ssh
8-1. ssh 접속 해제
exit
8-2. vm 전원 끔
vagrant halt
9. vm에 git 설치
sudo yum install git -y (-y 옵션주면 자동으로 y입력)
10. git 폴더 생성
mkdir git
11. git 폴더 접속
cd git
12. local repository 생성
git clone repository주소
12-1. 잘못 설치했을 경우
rm -rf repository주소 (-rf 옵션주면 강제 제거)
13. git에 user name & user email config
git config --global user.name "이름"
git config --global user.email "이메일"
14. nano 설치
sudo yum install nano -y
15. nano로 README.md 파일 수정
nano README.md
15-1. nano 에디터 편집하기
저장하기 : Ctrl + O 입력 후 Enter 입력
나가기 : Ctrl + X
16. 수정 내용 staged
git add .
17. 수정 내용 local repository에 commit
git commit -m "기록 내용"
18. 수정 내용 remote repository에 push
git push
