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


Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile/vprofile-project/vagrant/Manual_provisioning (local-setup)
# $ vagrant plugin install vagrant-hostmanager

# $ vagrant plugin install vagrant-hostmanager
Installing the 'vagrant-hostmanager' plugin. This can take a few minutes...
Fetching vagrant-hostmanager-1.8.9.gem
Installed the plugin 'vagrant-hostmanager (1.8.9)'!


Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile/vprofile-project (local-setup)
# $ vagrant up
Bringing machine 'web01' up with 'virtualbox' provider...
Bringing machine 'app01' up with 'virtualbox' provider...
Bringing machine 'rmq01' up with 'virtualbox' provider...
Bringing machine 'mc01' up with 'virtualbox' provider...
Bringing machine 'db01' up with 'virtualbox' provider...
==> web01: Box 'ubuntu/bionic64' could not be found. Attempting to find and inst
    web01: Box Provider: virtualbox
    web01: Box Version: >= 0
==> web01: Loading metadata for box 'ubuntu/bionic64'
    web01: URL: https://vagrantcloud.com/ubuntu/bionic64
==> web01: Adding box 'ubuntu/bionic64' (v20230303.0.0) for provider: virtualbox
    web01: Downloading: https://vagrantcloud.com/ubuntu/boxes/bionic64/versions/albox.box
Download redirected to host: cloud-images.ubuntu.com
    web01:
==> web01: Successfully added box 'ubuntu/bionic64' (v20230303.0.0) for 'virtual
==> web01: Importing base box 'ubuntu/bionic64'...
==> web01: Matching MAC address for NAT networking...
==> web01: Checking if box 'ubuntu/bionic64' version '20230303.0.0' is up to dat
==> web01: Setting the name of the VM: Manual_provisioning_web01_1678786956050_1
==> web01: Clearing any previously set network interfaces...
==> web01: Preparing network interfaces based on configuration...
    web01: Adapter 1: nat
    web01: Adapter 2: hostonly
==> web01: Forwarding ports...
    web01: 22 (guest) => 2222 (host) (adapter 1)
==> web01: Running 'pre-boot' VM customizations...
==> web01: Booting VM...
==> web01: Waiting for machine to boot. This may take a few minutes...
    web01: SSH address: 127.0.0.1:2222
    web01: SSH username: vagrant
    web01: SSH auth method: private key
    web01: Warning: Connection reset. Retrying...
    web01: Warning: Connection aborted. Retrying...
    web01:
    web01: Vagrant insecure key detected. Vagrant will automatically replace
    web01: this with a newly generated keypair for better security.
    web01:
    web01: Inserting generated public key within guest...
    web01: Removing insecure key from the guest if it's present...
    web01: Key inserted! Disconnecting and reconnecting using new SSH key...
==> web01: Machine booted and ready!
==> web01: Checking for guest additions in VM...
    web01: The guest additions on this VM do not match the installed version ofrsion of                                                                can
    web01: VirtualBox! In most cases this is fine, but in rare cases it If you s can                                                                   ithin the
    web01: prevent things such as shared folders from working properly.talled on If you see
    web01: shared folder errors, please make sure the guest additions within the
    web01: virtual machine match the version of VirtualBox you have installed on
    web01: your host and reload your VM.
    web01:
    web01: Guest Additions Version: 5.2.42                             roject/va
    web01: VirtualBox Version: 7.0
==> web01: Setting hostname...
==> web01: Configuring and enabling network interfaces...
==> web01: Mounting shared folders...
    web01: /vagrant => C:/Users/Zakaria/devops_teli/vprofile/vprofile-project/vale-project/vagrant/Manual_provisioning
==> web01: [vagrant-hostmanager:guests] Updating hosts file on active guest virtve guest virtual machines...
==> web01: [vagrant-hostmanager:host] Updating hosts file on your workstation (porkstation (password may be required)...
==> app01: Importing base box 'geerlingguy/centos7'...
==> app01: Matching MAC address for NAT networking...
==> app01: Checking if box 'geerlingguy/centos7' version '1.2.27' is up to date...
==> app01: Setting the name of the VM: Manual_provisioning_app01_1678787094448_62487
==> app01: Fixed port collision for 22 => 2222. Now on port 2200.
==> app01: Clearing any previously set network interfaces...
==> app01: Preparing network interfaces based on configuration...
    app01: Adapter 1: nat
    app01: Adapter 2: hostonly
==> app01: Forwarding ports...
    app01: 22 (guest) => 2200 (host) (adapter 1)
==> app01: Running 'pre-boot' VM customizations...
==> app01: Booting VM...
==> app01: Waiting for machine to boot. This may take a few minutes...
    app01: SSH address: 127.0.0.1:2200
    app01: SSH username: vagrant
    app01: SSH auth method: private key
    app01:
    app01: Vagrant insecure key detected. Vagrant will automatically replace
    app01: this with a newly generated keypair for better security.
    app01:
    app01: Inserting generated public key within guest...
    app01: Removing insecure key from the guest if it's present...
    app01: Key inserted! Disconnecting and reconnecting using new SSH key...
==> app01: Machine booted and ready!
==> app01: Checking for guest additions in VM...
    app01: The guest additions on this VM do not match the installed version of
    app01: VirtualBox! In most cases this is fine, but in rare cases it can
    app01: prevent things such as shared folders from working properly. If you see
    app01: shared folder errors, please make sure the guest additions within the
    app01: virtual machine match the version of VirtualBox you have installed on
    app01: your host and reload your VM.
    app01:
    app01: Guest Additions Version: 6.1.32
    app01: VirtualBox Version: 7.0
==> app01: Setting hostname...
==> app01: Configuring and enabling network interfaces...
==> app01: Mounting shared folders...
    app01: /vagrant => C:/Users/Zakaria/devops_teli/vprofile/vprofile-project/vagrant/Manual_provisioning
==> app01: [vagrant-hostmanager:guests] Updating hosts file on active guest virtual machines...
==> app01: [vagrant-hostmanager:host] Updating hosts file on your workstation (password may be required)...
==> rmq01: Importing base box 'geerlingguy/centos7'...
==> rmq01: Matching MAC address for NAT networking...
==> rmq01: Checking if box 'geerlingguy/centos7' version '1.2.27' is up to date...
==> rmq01: Setting the name of the VM: Manual_provisioning_rmq01_1678787202762_20356
==> rmq01: Fixed port collision for 22 => 2222. Now on port 2201.
==> rmq01: Clearing any previously set network interfaces...
==> rmq01: Preparing network interfaces based on configuration...
    rmq01: Adapter 1: nat
    rmq01: Adapter 2: hostonly
==> rmq01: Forwarding ports...
    rmq01: 22 (guest) => 2201 (host) (adapter 1)
==> rmq01: Booting VM...
==> rmq01: Waiting for machine to boot. This may take a few minutes...
    rmq01: SSH address: 127.0.0.1:2201
    rmq01: SSH username: vagrant
    rmq01: SSH auth method: private key
    rmq01:
    rmq01: Vagrant insecure key detected. Vagrant will automatically replace
    rmq01: this with a newly generated keypair for better security.
    rmq01:
    rmq01: Inserting generated public key within guest...
    rmq01: Removing insecure key from the guest if it's present...
    rmq01: Key inserted! Disconnecting and reconnecting using new SSH key...
==> rmq01: Machine booted and ready!
==> rmq01: Checking for guest additions in VM...
    rmq01: The guest additions on this VM do not match the installed version of
    rmq01: VirtualBox! In most cases this is fine, but in rare cases it can
    rmq01: prevent things such as shared folders from working properly. If you see
    rmq01: shared folder errors, please make sure the guest additions within the
    rmq01: virtual machine match the version of VirtualBox you have installed on
    rmq01: your host and reload your VM.
    rmq01:
    rmq01: Guest Additions Version: 6.1.32
    rmq01: VirtualBox Version: 7.0
==> rmq01: Setting hostname...
==> rmq01: Configuring and enabling network interfaces...
==> rmq01: Mounting shared folders...
    rmq01: /vagrant => C:/Users/Zakaria/devops_teli/vprofile/vprofile-project/vagrant/Manual_provisioning
==> rmq01: [vagrant-hostmanager:guests] Updating hosts file on active guest virtual machines...
==> rmq01: [vagrant-hostmanager:host] Updating hosts file on your workstation (password may be required)...
==> mc01: Importing base box 'geerlingguy/centos7'...
==> mc01: Matching MAC address for NAT networking...
==> mc01: Checking if box 'geerlingguy/centos7' version '1.2.27' is up to date...
==> mc01: Setting the name of the VM: Manual_provisioning_mc01_1678787304457_99811
==> mc01: Fixed port collision for 22 => 2222. Now on port 2202.
==> mc01: Clearing any previously set network interfaces...
==> mc01: Preparing network interfaces based on configuration...
    mc01: Adapter 1: nat
    mc01: Adapter 2: hostonly
==> mc01: Forwarding ports...
    mc01: 22 (guest) => 2202 (host) (adapter 1)
==> mc01: Booting VM...
==> mc01: Waiting for machine to boot. This may take a few minutes...
    mc01: SSH address: 127.0.0.1:2202
    mc01: SSH username: vagrant
    mc01: SSH auth method: private key
    mc01: Warning: Connection reset. Retrying...
    mc01:
    mc01: Vagrant insecure key detected. Vagrant will automatically replace
    mc01: this with a newly generated keypair for better security.
    mc01:
    mc01: Inserting generated public key within guest...
    mc01: Removing insecure key from the guest if it's present...
    mc01: Key inserted! Disconnecting and reconnecting using new SSH key...
==> mc01: Machine booted and ready!
==> mc01: Checking for guest additions in VM...
    mc01: The guest additions on this VM do not match the installed version of
    mc01: VirtualBox! In most cases this is fine, but in rare cases it can
    mc01: prevent things such as shared folders from working properly. If you see
    mc01: shared folder errors, please make sure the guest additions within the
    mc01: virtual machine match the version of VirtualBox you have
installed on
    mc01: your host and reload your VM.
    mc01:
    mc01: Guest Additions Version: 6.1.32
    mc01: VirtualBox Version: 7.0
==> mc01: Setting hostname...
==> mc01: Configuring and enabling network interfaces...
==> mc01: Mounting shared folders...
    mc01: /vagrant => C:/Users/Zakaria/devops_teli/vprofile/vprofile-project/vagrant/Manual_provisioning
==> mc01: [vagrant-hostmanager:guests] Updating hosts file on active guest virtual machines...
==> mc01: [vagrant-hostmanager:host] Updating hosts file on your workstation (password may be required)...
==> db01: Importing base box 'geerlingguy/centos7'...
==> db01: Matching MAC address for NAT networking...
==> db01: Checking if box 'geerlingguy/centos7' version '1.2.27' is up to date...
==> db01: Setting the name of the VM: Manual_provisioning_db01_1678787415671_56991
==> db01: Fixed port collision for 22 => 2222. Now on port 2203.
==> db01: Clearing any previously set network interfaces...
==> db01: Preparing network interfaces based on configuration...
    db01: Adapter 1: nat
    db01: Adapter 2: hostonly
==> db01: Forwarding ports...
    db01: 22 (guest) => 2203 (host) (adapter 1)
==> db01: Booting VM...
==> db01: Waiting for machine to boot. This may take a few minutes.
This may take a few minutes...
    db01: SSH address: 127.0.0.1:2203
    db01: SSH username: vagrant
    db01: SSH auth method: private key
    db01: Warning: Connection aborted.
Retrying...
    db01: Warning: Connection reset. Retrying...
    db01:
    db01: Vagrant insecure key detected. Vagrant will automatically replace
    db01: this with a newly generated keypair for better security.
    db01:
    db01: Inserting generated public key within guest...
    db01: Removing insecure key from the guest if it's present...
    db01: Key inserted! Disconnecting and reconnecting using new SSH key...
==> db01: Machine booted and ready!
==> db01: Checking for guest additions
in VM...
    db01: The guest additions on this VM do not match the installed version of    db01: VirtualBox! In most cases this is fine, but in rare cases it can
    db01: prevent things such as shared folders from working properly. If you
see
    db01: shared folder errors, please
make sure the guest additions within the
    db01: virtual machine match the version of VirtualBox you have installed on
    db01: your host and reload your VM.    db01:
    db01: Guest Additions Version: 6.1.32
    db01: VirtualBox Version: 7.0
==> db01: Setting hostname...
==> db01: Configuring and enabling network interfaces...ork interfaces...
==> db01: Mounting shared folders...   devops_teli/vprofile/vprofile-project/vagrant/Manual_provisioning
    db01: /vagrant => C:/Users/Zakaria/Updating hosts file on active guest virtual machines...devops_teli/vprofile/vprofile-project/vdating hosts file on your workstation (password may be required)...agrant/Manual_provisioning
==> db01: [vagrant-hostmanager:guests] rofile/vprofile-project/vagrant/Manual_provisioning (local-setup)
Updating hosts file on active guest virtual machines...
==> db01: [vagrant-hostmanager:host] Updating hosts file on your workstation (password may be required)...

Zakaria@Gen▒ve MINGW64 ~/devops_teli/vprofile/vprofile-project/vagrant/Manual_provisioning (local-setup)
$
