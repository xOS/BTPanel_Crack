# 宝塔面板破解
> 目前最新版7.5.2可用
## 操作
* html文件替换路径：
```bash
/www/server/panel/BTPanel/templates/default
```
* python文件替换路径：
```bash
/www/server/panel/class
```
* 然后执行：
```bash
sed -i "s|if (bind_user == 'True') {|if (bind_user == 'REMOVED') {|g" /www/server/panel/BTPanel/static/js/index.js
chattr +i /www/server/panel/class/panelPlugin.py
chattr +i /www/server/panel/BTPanel/templates/default/index.html
chattr +i /www/server/panel/BTPanel/static/js/index.js
```
* 重启宝塔
* 强制刷新浏览器缓存
* OK
