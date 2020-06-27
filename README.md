# Docker image building
docker build -t daya123/nginx6 .

build -t daya123/nginx6 .

$ vi Dockerfile
$ docker build -t daya123/nginx6 . 
$ docker images
$ docker push daya123/nginx6

# To upload for git web
```
user@DAYA MINGW64 ~/MSC (master)
$ echo "# MSC" >> README.md

user@DAYA MINGW64 ~/MSC (master)
$ git init
Reinitialized existing Git repository in C:/Users/user/MSC/.git/

user@DAYA MINGW64 ~/MSC (master)
$ git add README.md

user@DAYA MINGW64 ~/MSC (master)
$ git commit -m "README.md Added"
[master 194d18a] README.md Added
 1 file changed, 1 insertion(+), 1 deletion(-)

user@DAYA MINGW64 ~/MSC (master)
$ git remote add origin https://github.com/onespace10/MSC.git

user@DAYA MINGW64 ~/MSC (master)
$ git push -u origin master
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 8 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (11/11), 269.48 KiB | 19.25 MiB/s, done.
Total 11 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/onespace10/MSC.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
```

# MSC
https://github.com/onespace10/MSC.git  # MSC
