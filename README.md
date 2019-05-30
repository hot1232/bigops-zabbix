# 给zabbix补丁，支持cas认证<br>
>cd zabbix-x.x.x<br/>
>patch -p1 < zabbix-x.x.x.patch<br>

**备注：制作patch**<br>
移动文件conf/zabbix.conf.php出要打patch的目录，然后执行命令<br>
>diff -Nuar old new > zabbix-x.x.x.patch<br>
移动文件conf/zabbix.conf.php回原处<br>

注意，这里的顺序一定是旧目录在前。<br>
