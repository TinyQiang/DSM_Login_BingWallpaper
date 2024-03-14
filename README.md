# DSM_Login_BingWallpaper
>  在这个项目上改的[DSM_Login_BingWallpaper](https://github.com/kkkgo/DSM_Login_BingWallpaper)

在原来脚本的基础上，增加一个文件用来记录执行次数。每执行一次就更换下一张Bing壁纸。  
这样可以设置成每小时执行一次，就每小时换一次壁纸。  
# 我本人不会脚本，修改脚本全靠文心一言提问来完成。  

# 注意
不要将代码直接写入到脚本处，执行可能会出错。  
  
# 将下载的脚本直接上传到群晖中
  
![脚本文件上传到群晖中.png](https://s2.loli.net/2024/03/15/SqAsFmlcK1Yp96B.jpg)
# 然后在计划任务中填写脚本的地址来执行脚本。
![脚本使用说明.png](https://s2.loli.net/2024/03/15/jKECAV2M3tnlqH4.jpg)
  
可以通过选中脚本，然后查看运行结果，正常运行应该和下来一样，就是数值不一样。
![查看脚本执行结果.png](https://s2.loli.net/2024/03/15/9iLoI84W2vyCblq.png)

# 增加修改应用登录背景图片的功能  
> 打开脚本，找到这一段
```sh
#修改应用程序登录壁纸，需要修的的就把对应的程序名前的#去掉
AudioStation=yes
DownloadStation=yes
FileStation=yes
SynologyDrive=yes
SynologyPhotos=yes
VideoStation=yes
```
这里默认是修改应用背景，如果不需要修改应用背景，则在对应的应用名称前面加上#号即可。  
> 如果没有效果，先在在群晖里面应用登录设置里面随便自定义选择一个壁纸，保存后再试。

# 登录框透明脚本
```sh
<style type="text/css"> .tab-panel {background: rgba(255,255,255,0.5) !important;} .login-textfield .input-container input { background-color: transparent !important; } body {-webkit-filter:brightness(1); -o-filter:brightness(1); -moz-filter:brightness(1); filter:brightness(1);} </style>
```
  
使用方法：  
将上面的脚本填入到登录样式的脚本信息里面，勾选以HTML语法显示。  
  
![登录框透明.png](https://s2.loli.net/2024/03/15/8pk4uiB9cHnwQVT.jpg)

# 效果
  
![修改后效果.png](https://s2.loli.net/2024/03/15/m2eDbp6hZAgvlOd.jpg)
