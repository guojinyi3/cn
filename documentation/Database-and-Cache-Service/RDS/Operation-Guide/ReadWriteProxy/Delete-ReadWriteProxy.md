# 关闭读写分离代理

当您的业务不再需要使用读写分离代理时， 您可以关闭读写分离代理。关闭读写分离代理不影响当前主实例和只读实例的功能，但读写分离代理的域名将会失效，您需要在在程序中重新配置主实例或只读实例的地址。

## 操作步骤
1. 登录 [云数据库 RDS 控制台](https://rds-console.jdcloud.com/database)。
2. 选择需要开启读写代理的目标实例，点击目标实例的名称，进入到实例详情页。
3. 选择 **读写代理** 标签，打开读写代理管理页面。
4. 点击 **关闭读写分离代理** 按钮，进入关闭读写分离代理提示页面。
    
   ![删除读写代理](../../../image/RDS/ReadWriteProxy-Delete.png)

5. 点击 **确定** 按钮，关闭读写分离代理。


