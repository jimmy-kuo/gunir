# gunir
Gunir is abbr. from Gungnir

# How to run Gunir

* Install blade:

        $ svn co https://svn.baidu.com/ps/se/trunk/offline/nearline/common/tools
        $ ./install_blade.sh

* download gunir from github：

        $ git clone https://github.com/anqin/gunir
        $ cd gunir
        $ ./get_internal_deps.sh


* compile gunir

        $ cd gunir/gunir
        $ blade build -pdebug :gunir_main

make sure the protobuf is version 2.4.1

* run the gunir

        $ cd deploy/onebox
        $ ./start_servers.sh <<-- start servers
        $ ./kill_servers.sh <<-- stop servers
        
        $./gunir_main --gunir_role=client --flagfile=gunir.flag   <<-- run client

Enjoy it~~
