#                                 企业门户网站

​     系统后端服务为nodejs开发，管理前端和门户网站使用vue3开发。目前功能已比较完善，首页banner轮播图支持自定义配置，各展示板块图文（栏目）样式支持多种选择，企业信息，如logo、企业介绍、企业文化、官方微信、联系方式等在管理端维护后自动展示在门户网站相应位置，管理端支持新闻资讯发布、产品发布、职位发布。

## 一、采用技术方案

该系统采用的主要技术如下：
1. [Vue.js](https://cn.vuejs.org/)
2. [Element Plus](https://element-plus.gitee.io/zh-CN/)
3. [axios](http://www.axios-js.com/zh-cn/docs/index.html)
4. [node.js](https://nodejs.org/zh-cn/docs/)
5. [Sequelize](https://www.sequelize.com.cn/)
6. [Koa](https://koa.bootcss.com/)
7. minio

## 二、开发环境

1. 操作系统：Windows10
2. 数据库：MySQL 5.7
3. Web服务器：Nginx 
4. 开发工具：Webstorm
5. 系统基础环境：Node.js

## 三、演示地址

1. 企业门户：http://www.farsailing.com

2. 管理后台：http://119.29.209.39:8200  账号：admin，密码：123456

## 四、目录说明

server---后端接口服务

admin---网站管理端

![WX20230705-141751@2x](images/WX20230705-141751@2x.png)

web---门户网站

首页：

![QQ20230818-110834@2x](images/QQ20230818-110834@2x.png)

![WechatIMG311](images/121.png)

产品页：

![QQ20230818-110834@2x](images/QQ20230818-111343@2x.png)

![WechatIMG314](images/WechatIMG314.png)

![QQ20230818-110834@2x](images/QQ20230818-111343@2x.png)

![WechatIMG316](images/WechatIMG316.png)

新闻资讯页：

![QQ20230818-110834@2x](images/QQ20230818-111453@2x.png)

![iShot_2023-07-06_14.15.58](images/iShot_2023-07-06_14.15.58.png)

关于我们：

![QQ20230818-111229@2x](images/QQ20230818-111229@2x.png)

## 五、如何本地运行

1. 先启动后端(server目录下)
```bash
yarn install

npm run start(本地启动)

或者 npm run dev(实时监听改动重启，边改边跑) 需要全局安装 nodemon
```
2. 启动前端（web 或者 admin目录下）
```bash
# 1.安装
npm install / yarn install
# 2.启动
npm run dev / yarn dev
# 3.打包
npm run build / yarn build
# 4.清除 node_modules
npm run clear / yarn clear
```
yarn命令请提前全局安装
```bash
npm i yarn -g
```

## 六、补充说明

1.cd到各自的目录下跑，系统分为门户网站、管理后台、后端接口服务三个项目，根目录无法直接运行。

2.请严格检查自己的node版本。鉴于已经发现的问题，在windows环境下，建议使用node 14的大版本；mac系统 14和16都OK(运行在APPLE M1之上)。

3.如果数据库连接报错，请首先检查server(后端node)下config目录中的dbinfo.js的配置与你自己的数据库配置是否正确。

4.图片文件等上传的资源使用minio存储，请自行百度搭建minio。

## 七、咨询

杨先生：

邮箱：[1041114134@qq.com](mailto:835487894@qq.com)

手机：15287192249

微信号：FinelyYang
