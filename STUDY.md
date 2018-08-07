<h1>Yii2 学习笔记 - HH</h1>

Advanced高级应用模板：[官方安装文档](https://github.com/yiisoft/yii2-app-advanced/blob/master/docs/guide/start-installation.md)

安装步骤：

- **Composer 安装** : 打开控制台，切换至Web根目录www。执行 'composer create-project --prefer-dist yiisoft/yii2-app-advanced yii-application' ，yii-application可修改为项目名称。

    1、打开控制台，切换至项目根目录yii-application，执行命令 php init ，选择dev开发模式。

    2、新建一个空数据库，依次打开项目文件/common/config/main-local.php,修改db数据库连接配置。
    
    3、打开控制台，切换至项目根目录yii-application，执行命令 php yii migrate 新增Advanced初始user
    表，另一个数据迁移表暂时不管。
    
> 至此，Advanced高级应用模板安装完毕。