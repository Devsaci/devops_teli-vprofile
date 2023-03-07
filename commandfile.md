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
