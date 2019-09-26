脚本运行完毕后，会显示 port 以及 psk，按照标准填入 Surge 即可。

![](https://scomper.me/_image/ssh-wget-snell.png)


** 请使用root用户运行 **

Centos & RedHat 用户
```
wget --no-check-certificate -O snell.sh https://raw.githubusercontent.com/ydzydzydz/snell.sh/master/snell.centos-port.sh
chmod +x snell.sh
./snell.sh
```

Debian & Ubuntu 用户
```
wget --no-check-certificate -O snell.sh https://raw.githubusercontent.com/ydzydzydz/snell.sh/master/snell-port.sh
chmod +x snell.sh
./snell.sh
```

卸载方法：
```
wget --no-check-certificate -O uninstall-snell.sh https://raw.githubusercontent.com/ydzydzydz/snell.sh/master/uninstall-snell.sh
chmod +x uninstall-snell.sh
./uninstall-snell.sh
```
运行状态
```
systemctl status snell
```
重启 Snell
```
systemctl restart snell
```
启动 Snell
```
systemctl start snell
```
停止 Snell
```
systemctl stop snell
```
----
查看 Snell 配置文件
```
cat /etc/snell/snell-server.conf
```
修改 Snell 配置文件
```
vi /etc/snell/snell-server.conf
```

