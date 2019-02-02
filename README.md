
## 简介

> react-juejin!

> 技术栈

- react全家桶
- ant design
- egg.js
- mysql

前后端分离开发模式，前端项目与后端项目属于不同的工程

```javascript
// instagram/client 前端工程
// instagram/service 后端工程
```






## 运行项目

因前后端不同端口原因，为解决跨域。前端工程启动了devServer，需先启动后端工程

* git clone https://github.com/zhoushaw/Instagram.git
* cd Instagram

> 运行后端项目

* 请确保本地已装mysql，并配置全局变量
* mysql -u root -p 并输入数据库密码
* create database learn; 创建learn数据库
* use learn;  切换数据库
* source learn.sql的路径; 例如：source /Users/shawzhou/Desktop/learning/instagram/db/learn.sql;
* 配置egg.js连接数据库信息

```javascript
// 前往service/config/config.local.ts，配置你的数据库信息
config.sequelize = {
    dialect: 'mysql',
    host: '127.0.0.1',
    port: 3306,
    database: 'learn',
    username: '', 
    password: '', 
    operatorsAliases: false
};
```


```


* 在/service文件下
* npm install
* npm run dev


> 运行前端项目

* cd client
* npm install
* npm start

## 目标功能

- [X] 登录、注册    -- 完成
- [X] 修改个人信息  --完成
- [X] 关注  -- 完成
- [X] 评论  -- 完成
- [X] 点赞  -- 完成
- [X] 搜索帖子  -- 完成
- [X] 上传头像  -- 完成
- [X] 发帖  -- 完成
- [X] 收藏  -- 未完成


> 如果对您有帮助，您可以点右上角 "Star" 支持一下 谢谢！ ^_^