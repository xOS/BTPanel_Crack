# 宝塔面板破解
> 目前最新版7.4.6可用
## 操作
* html文件替换路径：
```bash
/www/server/panel/BTPanel/templates/default
```
* python文件替换路径：
```bash
/www/server/panel/class
```
* 删除文件 
```bash
/www/server/panel/BTPanel/static/js/index.js 
```
第 65-67 行：
```bash
if (bind_user == 'True') {
    show_force_bind();
}
```
* 然后执行：
```bash
chattr +i /www/server/panel/class/panelPlugin.py
chattr +i /www/server/panel/BTPanel/templates/default/index.html
chattr +i /www/server/panel/BTPanel/static/js/index.js
```
* 重启宝塔
* 强制刷新浏览器缓存
* OK
