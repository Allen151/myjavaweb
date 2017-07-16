# tomcat的使用  
tomcat的安装版本是在安装的过程中选择jdk的路径的，而压缩版本是在安装完成后在环境变量的配置时候选择jkd的路径的。认识到这点安装就不会有什么问题了。  
### 改变端口号  
在tomcat的安装目录`D:\ProgramFiles\Apache Software Foundation\Tomcat 8.5\conf`下找到`server.xml`文件，以下代码是端口号：将8080改成你需要的端口号即可，要重启tomcat更改才生效
```html
<Connector port="8080" protocol="HTTP/1.1"
               connectionTimeout="20000"
               redirectPort="8443" />
```

## 第三课  
1.使用JavaEE版的Eclipse开发动态的WEB工程（javaWEB项目）  
1).把开发选项切换到JavaEE  
2).可以在Window-》Show View中找到Package Explorer，并拖其出来放好供使用。  
3).在Servers面板中新建Tomcat服务器，一定要关联到Tomcat安装的要目录下。  
4).新建一个Dynamic Web Project。其中Target Runtime需要选项好tomcat的版本。  
5).开发java Web应该  
6).可以通过run on server 来运行WEB项目