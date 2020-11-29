# HBuilder X搭建php环境

## 1.安装好phpstudy

百度下载 php集成环境:phpstudy

比如:集成环境工具安装在这路径:C:\phpstudy_pro

菜单栏 左边 环境.安装好php插件

然后在工具首页,点击 一键启动:WNMP启动



## 2.设置:外部浏览器调用url:

在HBuilder工具里面顶部----运行---运行到浏览器---配置web服务器

设置:外部浏览器调用url:

http://127.0.0.1:80



## 3.导入文件

（注意注意只有在phpstudy_pro\WWW下的文件才能运行，php html文件也是一样）

HBuilder工具里面顶部---文件----导入-----从本地目录导入:在集成环境安装目录里面选中网站的目录:C:\phpstudy_pro\WWW

然后在C:\phpstudy_pro\WWW 这个目录里面新建一个2.php文件。



## 4.预览网页

HBuilder X右上角点击预览，选择PC模式

在php文件里边输以下代码，再刷新即可预览

```php
<?php
    $a=134;
    echo $a;
?>
```

右边的网址全部复制到其他浏览器打开也能预览。

目前在HBuilder X的web浏览器预览发现一个小bug，预览html文件是alert(“&”);一个&不显示，实际上已经有一个“&”了。

alert(“&&”);才会显示一个，另一个被隐藏。console.log("&");可以一个不漏的打印出来。

如果遇到有类似问题，建议复制网址去其他浏览器打开。

