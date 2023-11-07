$ git init
Initialized empty Git repository in C:/Users/Admin/Desktop/cdv0063/.git/

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (master)
$ git remote add origin "https://github.com/vasanthe123/assignment.git"

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (master)
$ notepad sample.txt

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (master)
$ git add .

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (master)
$ git commit -m "first commit in master"
[master (root-commit) eca0405] first commit in master
 1 file changed, 2 insertions(+)
 create mode 100644 sample.txt

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (master)
$ git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 244 bytes | 122.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/vasanthe123/assignment.git
 * [new branch]      master -> master

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (master)
$ git branch feature-branch

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (master)
$ git checkout feature-branch
Switched to branch 'feature-branch'

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (feature-branch)
$ notepad sample.txt

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (feature-branch)
$ git add .

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (feature-branch)
$ git commit -m "first commit in feature branch"
[feature-branch 39c7216] first commit in feature branch
 1 file changed, 3 insertions(+), 1 deletion(-)

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (feature-branch)
$ git push origin feature-branch
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 302 bytes | 151.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'feature-branch' on GitHub by visiting:
remote:      https://github.com/vasanthe123/assignment/pull/new/feature-branch
remote:
To https://github.com/vasanthe123/assignment.git
 * [new branch]      feature-branch -> feature-branch

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (feature-branch)
$ git checkout master
Switched to branch 'master'

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (master)
$ git merge feature-branch
Updating eca0405..39c7216
Fast-forward
 sample.txt | 4 +++-
 1 file changed, 3 insertions(+), 1 deletion(-)

Admin@DESKTOP-N872A1D MINGW64 ~/Desktop/cdv0063 (master)
$ git push origin master
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/vasanthe123/assignment.git
   eca0405..39c7216  master -> master
