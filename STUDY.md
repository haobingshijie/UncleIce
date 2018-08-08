<h1>Yii2 学习笔记 - HH</h1>

Advanced高级应用模板：[官方安装文档](https://github.com/yiisoft/yii2-app-advanced/blob/master/docs/guide/start-installation.md)

安装步骤：

- **Composer 安装** : 打开控制台，切换至Web根目录www。执行` composer create-project --prefer-dist yiisoft/yii2-app-advanced yii-application` ，yii-application可修改为自己的项目名称。

    1、打开控制台，切换至项目根目录yii-application，执行命令 php init ，选择dev开发模式。

    2、新建一个空数据库，依次打开项目文件/common/config/main-local.php,修改db数据库连接配置。
    
    3、打开控制台，切换至项目根目录yii-application，执行命令 php yii migrate 新增Advanced初始user
    表，另一个数据迁移表暂时不管。
    
> 至此，Advanced高级应用模板安装完毕。

Advanced目录结构：
```
frontend与backend
前后台入口，都有着各自的【MVC目录(models|views|controllers)、配置文件目录(config)、入口文件目录(web)、资源文件目录(assets)】。

console
控制台入口，用来控制执行的程序，比如放一些定时执行的程序，或者需要在更底层的操作系统上运行的功能。

common
共用的目录，比如前后台共用的模型文件就可以放在这里。

environments
放环境的配置文件。
```

__ DIR __ 返回当前文件的目录:
```
    eg: D:\wamp\WWW\phpinfo.php
        echo __DIR__;
        D:\wamp\WWW
```

dirname() 返回当前文件路径的上一级:
```
    eg: D:\wamp\WWW\phpinfo.php
        1.
            echo dirname('D:\wamp\WWW\phpinfo.php');
            D:\wamp\WWW
        2.  echo dirname(__DIR__);
            D:\wamp
```