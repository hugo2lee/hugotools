# hugotools
tao tools

20161215-linux新建执行脚本：nano run.sh > # !/bin/sh nano down_page.py 保存后 bash run.sh 运行
         linux快速进入某个文件夹：在 home 里的 .bashrc 添加 alias zno = 'cd /home/hugo/web/0and1' 然后执行一下source ~/.bashrc 
                                  以后直接 输入 zno 就直接打开 0and1 了
20161216-ubuntu16 打开mysql远程访问：1编辑mysql配置文件，把/etc/mysql/mysql.conf.d/mysqld.cnf 其中bind-address = 127.0.0.1注释了
                                     2mysql> use mysql; 
                                      mysql> update user set host = '%' where user = 'root'; 
                                      mysql> select host, user from user; 
                                      mysql> flush privileges;
