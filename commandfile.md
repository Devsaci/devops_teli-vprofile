Zakaria@Gen▒ve MINGW64 ~
# $ cd devops_teli

Zakaria@Gen▒ve MINGW64 ~/devops_teli

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile
# $ git init
Initialized empty Git repository in C:/Users/Zakaria/devops_teli/vprofile/.git/

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile (master)
# $ touch commandfile.md

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile (master)
# $ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        commandfile.md

nothing added to commit but untracked files present (use "git add" to track)

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile (master)
# $ git add .

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile (master)
# $ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   commandfile.md


Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile (master)
# $ git commit -m"init vprofile project & commandfile.md"
[master (root-commit) e723b30] init vprofile project & commandfile.md
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 commandfile.md

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile (master)

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile (master)
# $ git clone https://github.com/devopshydclub/vprofile-project/tree/local-setup/vagrant/Manual_provisioning
Cloning into 'Manual_provisioning'...
fatal: repository 'https://github.com/devopshydclub/vprofile-project/tree/local-setup/vagrant/Manual_provisioning/' not found

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile (master)
# $ git clone https://github.com/devopshydclub/vprofile-project.git
Cloning into 'vprofile-project'...
remote: Enumerating objects: 2644, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (5/5), done.

Receiving objects: 100% (2644/2644), 75.71 MiB | 2.19 MiB/s, done.
Resolving deltas: 100% (966/966), done.

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile (master)
# $ ls
commandfile.md  vprofile-project

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile (master)
# $ cd vprofile-project

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile/vprofile-project (vp-rem)
# $ ls
ansible  files  Jenkinsfile  pom.xml  README.md  src

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile/vprofile-project (vp-rem)
# $ ls -al
total 25
drwxr-xr-x 1 Zakaria 197121    0 Mar  7 11:14 .
drwxr-xr-x 1 Zakaria 197121    0 Mar  7 11:13 ..
drwxr-xr-x 1 Zakaria 197121    0 Mar  7 11:14 .git
drwxr-xr-x 1 Zakaria 197121    0 Mar  7 11:14 ansible
drwxr-xr-x 1 Zakaria 197121    0 Mar  7 11:14 files
-rw-r--r-- 1 Zakaria 197121 4057 Mar  7 11:14 Jenkinsfile
-rw-r--r-- 1 Zakaria 197121 7522 Mar  7 11:14 pom.xml
-rw-r--r-- 1 Zakaria 197121  542 Mar  7 11:14 README.md
drwxr-xr-x 1 Zakaria 197121    0 Mar  7 11:14 src

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile/vprofile-project (vp-rem)
# $ git status
On branch vp-rem
Your branch is up to date with 'origin/vp-rem'.

nothing to commit, working tree clean

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile/vprofile-project (vp-rem)
# $ git checkout local-setup
Switched to a new branch 'local-setup'
branch 'local-setup' set up to track 'origin/local-setup'.

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile/vprofile-project (local-setup)
# $ ls
ansible  Jenkinsfile  pom.xml  README.md  src  vagrant

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile/vprofile-project (local-setup)
# $ cd vagrant

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile/vprofile-project/vagrant (local-setup)
# $ ls
Automated_provisioning  Automated_provisioning_MacOSM1  Manual_provisioning  Manual_provisioning_MacOSM1

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile/vprofile-project/vagrant (local-setup)
$