# 초보 개발자의 개발 일지
------------

* #### name : 이예찬
* #### email : 11chan11@naver.com

-------

<a href = "https://www.navercloudcorp.com/" target = "_blank">
        <img src = "./202209290853594643582.png" alt = "ncloud"/></a> AIaaS 개발자 과정 1기<br>

---

3차 실습<br>
vagrant 설치 & vm 생성 & 리눅스 설치 & git 설치 & nano 설치 & git 초기 설정<br>

1. 홈폴더에 vm-projects폴더 생성<br>
mkdir vm-projects<br>
2. vm-projects 폴더 접속<br>
cd vm-projects<br>
3. centos 폴더 생성<br>
mkdir centos<br>
4. centos 폴더 접속<br>
cd centos<br>
5. centos 이미지 파일 다운로드<br>
vagrant init "centos/7"<br>
6. vagrantfile에서 config.vm.hostname = "myhost5.bitcamp" 입력<br>
7. vagrant 설정 파일 다운로드 및 실행<br>
vagrant up<br>
8. vm에서 ssh로 접속<br>
vagrant ssh<br>
8-1. ssh 접속 해제<br>
exit<br>
8-2. vm 전원 끔<br>
vagrant halt<br>
9. vm에 git 설치<br>
sudo yum install git -y (-y 옵션주면 자동으로 y입력)<br>
10. git 폴더 생성<br>
mkdir git<br>
11. git 폴더 접속<br>
cd git<br>
12. local repository 생성<br>
git clone repository주소<br>
12-1. 잘못 설치했을 경우<br>
rm -rf repository주소 (-rf 옵션주면 강제 제거)<br>
13. git에 user name & user email config<br>
git config --global user.name "이름"<br>
git config --global user.email "이메일"<br>
14. nano 설치<br>
sudo yum install nano -y<br>
15. nano로 README.md 파일 수정<br>
nano README.md<br>
15-1. nano 에디터 편집하기<br>
저장하기 : Ctrl + O 입력 후 Enter<br>
입력 나가기 : Ctrl + X<br>
16. 수정 내용 staged<br>
git add .<br>
17. 수정 내용 local repository에 commit<br>
git commit -m "기록 내용"<br>
18. 수정 내용 remote repository에 push<br>
git push<br>

---

centos test
