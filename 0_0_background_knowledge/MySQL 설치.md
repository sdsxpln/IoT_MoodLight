## 설치 가능한 MySQL 버전 확인


> sudo apt-cache search mysql-server


![mysql_1](../0_1_img/mysql/1.png)


## MySQL 설치


**확인한 버전대로 설치해야함!!**


> sudo apt-get install mysql-server-5.7


![mysql_2](../0_1_img/mysql/2.PNG)


**리눅스에서는 비밀번호 입력할 때 입력하고 있는 글자가 표시되지 않음**


## MySQL 설치 확인

> mysql -uroot -p


![mysql_3](../0_1_img/mysql/3.PNG)


> exit


## 깃 설치


> sudo apt-get install git


## 커뮤니팁스 깃헙에서 프로젝트 파일 클론하기


> cd ~


> git clone https://github.com/Communitips/IoT_MoodLight.git


## MySQL 백업 파일 복구하기


> mysql -uroot -p


> CREATE DATABASE SensorNode;


> SHOW DATABASES;


![mysql_4](../0_1_img/mysql/4.png)


> mysql -uroot -p SensorNode < ~/IoT_MoodLight/nodejs/db/SensorNode.sql


## MySQL 복구 확인


> mysql -uroot -p


> use SensorNode;


> SELECT * FROM Temperature;


![mysql_5](../0_1_img/mysql/5.png)


위 사진처럼 어떤 값이 뜬다면 성공.(테이블 수정 중이라 값의 형태는 그림과 다를 수 있음.)
