# Docker image building
```
docker build -t daya123/nginx6 .

$ vi Dockerfile
$ docker build -t daya123/nginx6 . 
$ docker images
$ docker push daya123/nginx6
```
# To upload for git web
```
1. Docker 생성, 실행, 업데이트 및 이미지ID 생성
user@DAYA MINGW64 ~/MSC (master)
$ docker build -t daya123/nginx5 .
Sending build context to Docker daemon  674.3kB
Step 1/4 : FROM ubuntu
 ---> 74435f89ab78
Step 2/4 : RUN apt update
 ---> Using cache
 ---> 6bdac41154fb
Step 3/4 : RUN apt install -y nginx
 ---> Running in 3888d12494f1
Step 4/4 : CMD [ "nginx", "-g", "daemon off;" ]
 ---> Running in 294a2655b9e8
Removing intermediate container 294a2655b9e8
 ---> Using cache
 ---> 4cf240b87489
Successfully built 4cf240b87489
Successfully tagged daya123/nginx5:latest

2. Container 생성
$ docker run -it 이미지명(daya123/nginx5) <- 실행 후 먹통되고 ps -a에 CONTAINER ID(12자리)와 IMAGE(daya123/nginx5), NAMES(elated_solomon) 생성됨

3. Container 실행
$ docker ps -a <- NAMES(elated_solomon) 확인
$ docker start elated_solomon

4. docker commit
$ docker images  <- REPOSITORY 확인
$ docker ps -a <- CONTAINER 확인
$ docker commit 60b5a511da6c daya123/nginx5:v1.0 <- IMAGE TAG 설정
sha256:2e58f0d29103fdcdb826d189e47d4f0897491a67b2fcf2e92c8a2efd31af827a

5. docker push
$ docker ps -a <- IMAGE 확인
$ docker push daya123/nginx5:v1.0
The push refers to repository [docker.io/daya123/nginx5]
2d4e894c4180: Pushed 
d9556a6301e2: Pushed
90a8fb996317: Layer already exists
05f3b67ed530: Layer already exists
ec1817c93e7c: Layer already exists
9e97312b63ff: Layer already exists
e1c75a5e0bfa: Layer already exists
v1.0: digest: sha256:f550f55a4b31aa379ec3c0f728e0c256659cdf3cc3f632b1d6a578a7c0347304 size: 1783

6. git clone
$ git clone https://github.com/onespace10/MSC.git

$ pwd  <-  /c/Users/user/MSC
$ git add -A
$ git commit
$ git push
$ touch README.md
$ vi README.md
$ git add -A
$ git commit -m "README.md added"
$ git push
```

# MSC
https://github.com/onespace10/MSC.git
