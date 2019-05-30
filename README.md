# 安装说明
### 打补丁，支持cas认证<br>
>cd zabbix-x.x.x<br/>
>patch -p1 < zabbix-x.x.x.patch<br>

### 编辑文件conf/sso.conf.php<br>
1、修改SALT变量为在页面：监控/设置/Zabbix API/密码salt 里的值<br>
>$SALT = 'xxxxxxxxxxxxxxxxxxxxxx';<br>

### 如果sso使用的是https协议
1、需要打开conf/sso.conf.php文件里头部注释的行，并注释http对应的行<br>
2、并且用include/phpCAS/CAS/Client.php.bak覆盖include/phpCAS/CAS/Client.php<br>
记得先备份<br>


