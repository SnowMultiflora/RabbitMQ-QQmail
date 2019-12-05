# RabbitMQ-QQmail
使用Spring-Boot，Spring-Boot-JPA，RabbitMQ，themleaf完成简单的用户登录demo,注册时发送QQ邮件

用户注册完后，数据库改用户的状态为0，此时是无法登陆的，需要点击激活连接将状态改为1，才可登录。

在注册时，系统向QQ邮箱发送激活连接的邮件。
