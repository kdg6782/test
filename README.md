# 도커 알아보기

+ 기본 명령어 (CLI) 연습하기
+ Dockerfile를 ```docker build``` 하기

1 도커 이미지 확인

docker image list
docker image ls
docker images


2 도커 컨테이너 실행 확인 

 docker ps 

3.도커 컨테이너 전체 확인 

docker ps -a


4. 도커 컨테이너 생성 하기

docker create -i --name ubt ubuntu:24.04


5. 도커 컨테이너 시작 하기

docker start 컨테이너 아이디 or 이름


6. 도커 컨테이너 삭제 

docker rm  컨테이너 id or 이름  -f 강제 로 지우는 옵션 docker re -f ubt  강제삭제

7. 도커 컨테이너 정지 

docker stop ubt 

 8. 도커 컨테이너 실행 

 docker run -d -it --name ubt ubuntu:24.04  만들고  실행

9. 


10.

FROM ubuntu:24.04

RUN apt-get update

RUN apt-get install -y apache2

EXPOSE 80

CMD ["apache2ctl", "-D", "FOREGROUND"]#   t e s t  
 