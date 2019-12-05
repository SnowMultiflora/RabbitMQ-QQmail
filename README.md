# RabbitMQ-QQmail

使用技术：Spring-Boot，Spring-Boot-JPA，RabbitMQ，themleaf...
功能：完成简单的用户登录demo,注册时发送QQ邮件

描述：用户注册完后，数据库改用户的状态为0，此时是无法登陆的，需要点击激活连接将状态改为1，才可登录。
      在注册时，系统向QQ邮箱发送激活连接的邮件。
系统结构：user-sys:消息生产者，实现用户的注册登录，发送邮件的功能，并向Queue发送信息
         msg-sys:消息消费者  监听queue中的注册信息
         email-sys:消息消费者  监听queue中的登录信息
