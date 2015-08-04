# gunir
Gunir is abbr. from Gungnir

# How to run Gunir

1. Install blade:
$ svn co https://svn.baidu.com/ps/se/trunk/offline/nearline/common/tools
$ ./install_blade.sh

2. download gunir from github：
$ git clone https://github.com/anqin/gunir
$ cd gunir
$ ./get_internal_deps.sh


3. compile gunir
$ cd gunir/gunir
$ blade build -pdebug :gunir_main

4. run the gunir
$ cd deploy/onebox
$ ./start_servers.sh <<-- start servers
$ ./kill_servers.sh <<-- stop servers

$./gunir_main --gunir_role=client --flagfile=gunir.flag   <<-- run client

Enjoy it~~
