# xampp

<https://blog.berfen.com/36.html>

因为本人也在使用这个软件，安装和使用都非常简单，而且可以配置多个网站项目供本地测试。
那么下面来给大家介绍怎么配置

1、首先修改C盘WINDOWS\system32\drivers\etc目录下的 hosts 文件，用编辑器打开（需要管理员运行权限），加入：
（是在文件的未尾加入）

127.0.0.1 <www.berfen.com>
127.0.0.1 blog.berfen.com
2、打开xampp\apache\conf\httpd.conf文件
搜索 “Include conf/extra/httpd-vhosts.conf”，确保前面没有 # 注释符，也就是确保引入了 vhosts 虚拟主机配置文件。
开启了httpd-vhosts.conf，默认的httpd.conf默认配置失效
（确保 httpd-vhosts.conf 文件里也开启了虚拟主机配置，见第3条）
访问此IP的域名将全部指向 vhosts.conf 中的第一个虚拟主机。（注意是第一个，详见第4）

3、在虚拟主机设置文件xampp\apache\conf\extra\httpd-vhosts.conf里设置：
取消 NameVirtualHost *:80 前面的 ##，这样就启用了 vhosts.conf ，默认的httpd.conf默认配置失效。虚拟主机配置将只设置在 httpd-vhosts.conf 里。
然后在httpd-vhosts.conf文件的最末添加

<VirtualHost *:80>
    DocumentRoot "D:/www/berfen"
    ServerName <www.berfen.com>
</VirtualHost>

<VirtualHost *:80>
    DocumentRoot "D:/www/blog"
    ServerName blog.berfen.com
</VirtualHost>
文件目录可自行更改

4、 设置完了第3条之后，你会发现访问 localhost直接指向到设置的 berfen 那个路径去了，这个问题在第2条有讲。也就是开启了 vhosts后，默认的 httpd 的配置就会失效了，默认的访问就指向到 vhosts 里的第一条设置去了。这时候你要把 localhost的目录配置给设置回来。

<VirtualHost *:80>
    DocumentRoot "D:/xampp/htdocs/"
    ServerName localhost
</VirtualHost>
至此，XAMPP 的虚拟主机设置完毕，现在 访问 localhost 还是原来的 XAMPP 的帮助指南，访问 <www.berfen.com> 将指向到绑定的 berfen 目录，访问 blog.berfen.com 将指向到绑定的 blog 目录。

5、接下来修改xampp\apache\conf\httpd.conf的httpd.conf文件
在文件里查找AllowOverride none，这个是防止网站出现403拒绝访问，下面的代码是允许所有请求
全部内容：

<Directory />
    AllowOverride none
    Require all denied
</Directory>
请改成：

<Directory />
    #AllowOverride none
    #Require all denied
    AllowOverride All
</Directory>
然后搜索DocumentRoot "D:/xampp/htdocs"，如果不是D盘，可以搜索前面的英文，一般在250那几行
将：

DocumentRoot "D:/xampp/htdocs"

<Directory "D:/xampp/htdocs">
改成你希望的网站根目录，比如我的是

DocumentRoot "D:/www"

<Directory "D:/www">
6、将你的网站项目放入刚刚的网站项目文件夹里，重启Apacher，访问站点就行了
注意：你系统的文件hosts 文件在开启xampp的时候，会自动屏蔽并替换原有的网站
如果你的是

127.0.0.1 <www.baidu.com>
开启xampp后，在该网站目录新建一个html并填写“这是这个测试”，访问www.baidu.com就会显示你刚刚填的字符
这也是个域名装逼的方法
