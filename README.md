![](https://img.dobbinsoft.com/static/banner.jpg)
---  

[![Release Version](https://img.shields.io/badge/release-4.0.0-brightgreen.svg)](https://gitee.com/iotechn/unimall) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://gitee.com/iotechn/unimall/pulls)


> **社区版**

Unimall 针对中小商户、企业和个人学习者开发。使用Java编码，采用SpringBoot3、Mybatis-Plus等易用框架，适合个人学习研究。同时支持单机部署、集群部署，中小商户企业可根据业务动态扩容。unimall使用uniapp前端框架，可同时编译到 微信小程序、H5、Android App、iOS App等几个平台，可为中小商户企业节约大量维护成本。也可支撑中小商户企业前期平台横扩需求。

Unimall社区版源码包含:

- Java 后端服务
  - unimall-runner: 启动器（打包打这个就行）
  - unimall-admin-api: 提供管理员管理系统的WebApi
  - unimall-app-api: 提供APP、小程序、H5用户请求的WebApi
  - unimall-biz: 提供通用业务代码
  - unimall-data: 提供数据模型以及数据访问层封装
    - Vue 前端页面
  - unimall-admin: 基于element-ui的后台管理页面
  - unimall-app: 基于uniapp的小程序、H5、APP前端代码

- sql: 数据库初始化SQL脚本

## About this repository 关于

- release: 已经发布的分支
- develop: 正在开发的分支
  - dev-v4: 此分支已经完全测试过，但还没上过生产，可直接使用


## Experience 体验

- Client

  - 扫描下面二维码体验不同终端 **（体验APP使用浏览器扫码）**

![qr](https://img.dobbinsoft.com/static/qr.jpg)

- Pages

![front](https://img.dobbinsoft.com/readme/FO001.jpg)

- Admin
  - 后台演示地址: [https://unimallv4.dobbinsoft.com](https://unimallv4.dobbinsoft.com)
  - 登录名:guest 密码:123456 验证码:666666 (guest仅有只读权限，无读配置权限)
- Pages

![front](https://img.dobbinsoft.com/readme/BO001.png)  
![front](https://img.dobbinsoft.com/readme/BO002.png)  
![front](https://img.dobbinsoft.com/readme/BO003.png)  
![front](https://img.dobbinsoft.com/readme/BO004.png)  
![front](https://img.dobbinsoft.com/readme/BO005.png)

## New Features (v4) 新特性v4
| 描述                           |  
|:-----------------------------|  
| - 框架： 升级到JDK21 + SpringBoot3 |

## New Features (v3) 新特性v3
| 描述 |  
|:--------|  
| - 框架： 支持对象、字段注解生成文档 |  
| - 框架： 添加数据库扩展 |  
| - 框架： 支持滑动窗口Api限流 |  
| - 框架： 对接腾讯云对象存储 |  
| - 框架： 支持开放平台 |  
| - 功能： 添加用户在线支付开通、续费VIP |  
| - 功能： 对接App支付宝在线支付 |  
| - 功能： 对接支持道宾云ERP进销存系统 ⭐ |  



## The Framework 架构

![framework](https://img.dobbinsoft.com/readme/Framework.jpg)


## Getting started 快速开始

服务器可根据自身业务来选购，单机环境推荐2C4G

##### 方式一： docker 运行

视频教程： https://www.bilibili.com/video/BV1db4y1e7Vi/

文档教程：[点击查看](./docs/docker.01.env.md)


##### 方式二（推荐）： 编译运行
视频教程：https://www.bilibili.com/video/BV1EL4y1J7w5/

文档教程🍭🍭🍭：[文档1](./docs/build.01.env.md) [文档2](./docs/build.02.backend.md) [文档3](./docs/build.03.front.md)



## Document 文档

##### 框架v4文档

| 依赖                                   | 解释                   |  
| -------------------------------------- | ---------------------- |
| [support](../../../dobbinfw-support)   | 支持包，非常重要的文档 |  
| [launcher](../../../dobbinfw-launcher) | 启动器，非常重要的文档 |  
| [dobbinfw](../../../dobbinfw) | 脚手架文档 |  
| [fw-pay](../../../matrix-pay) | 支付文档 |  

## Copyright 版权

本项目后端由重庆驽驹科技有限公司开发，您可以在以任何方式部署或修改源代码。


![证书](https://img.dobbinsoft.com/static/UnimallCert.jpg)

前端代码使用的 mix.R 的开源模板，在此模板的基础上对接了Unimall后端Api，作者说不做商用限制，保留原地址，所以授权仅针对后端代码商用授权。

mix模板地址：https://ext.dcloud.net.cn/plugin?id=200

## Service 服务

##### 一、项目定制开发服务

若需要软件需求外包，小程序、App、网站、微信定制开发，请联系微信：dobbinsoft（请备注意图）

##### 二、电商小程序 SaaS 服务 (无代码快速上线微信小程序)

对于缺少技术的创业团队来说，使用SaaS服务即可解决掉技术问题。简单的说，就是由我们为客户统一运维，每年付一定的钱给我们就行了。

Unimall SaaS版每年980元。这个价格就和服务器的价格差不多。

使用Unimall SaaS版功能对比：


| 功能               | Unimall 开源版       | Unimall Pro SaaS |  
|------------------|-------------------|------------------|  
| 拖拽功能布局           | ❌                 | ✅                | 
| 主题引用（一键引入自己行业主题） | ❌                 | ✅                | 
| 商品管理             | ✅                 | ✅                |  
| 订单管理             | ✅                 | ✅                |  
| 运费模板             | ✅                 | ✅                |  
| O2O骑手配送          | ❌                 | ✅                |  
| 云订单打印 直接出小票      | ❌                 | ✅                |  
| 商品团购             | ✅                 | ✅                |  
| 优惠券              | ✅                 | ✅                |  
| 页面广告配置           | ✅                 | ✅                |  
| 类目管理             | ✅                 | ✅                |  
| 三级分销（渠道分销）       | ❌                 | ✅                |  
| 用户分销 用户推广获得返佣    | ❌                 | ✅                |  
| 好友砍价 邀请好友砍价      | ❌                 | ✅                |  
| 商品秒杀             | ❌                 | ✅                |  
| 积分 签到/购买商品 获取积分  | ❌                 | ✅                |  
| VIP卡 以VIP价格购买    | ✅                 | ✅                |  
| 服务商品-扫码核销        | ❌                 | ✅                |  
| 服务商品-资源编排        | ❌                 | ✅                | 
| 专属客服             | ❌                 | ✅                | 
| 系统优化（不另收费）       | ❌                 | ✅                |
| 费用               | 免费商用（不可二次出售或再次开源） | 980/年 无需服务器费用    |


支持试用：https://console.dobbinsoft.com/

注册账号，即可免费试用，试用规则： 未上线，不记时间，上线后，可免费试用7天。

## Contributing 贡献

如果你有好的意见或建议，欢迎给我们提 Issues 或 Pull Requests，为Unimall开源商城贡献力量。关于分支/issue及PR。


## 本地部署指南

### 环境准备

| 软件 | 版本要求 | 官网链接 |
|:-----|:---------|:---------|
| JDK | 21+ | [https://www.oracle.com/java/technologies/downloads/](https://www.oracle.com/java/technologies/downloads/) |
| MySQL | 5.7+ | [https://dev.mysql.com/downloads/](https://dev.mysql.com/downloads/) |
| Redis | 5.0+ | [https://redis.io/download/](https://redis.io/download/) |
| Maven | 3.8+ | [https://maven.apache.org/download.cgi](https://maven.apache.org/download.cgi) |
| Node.js | 14+ | [https://nodejs.org/en/download/](https://nodejs.org/en/download/) |
| HBuilderX（可选） | 最新版 | [https://www.dcloud.io/hbuilderx.html](https://www.dcloud.io/hbuilderx.html) |

### 环境搭建步骤

#### 1. 安装JDK

1. 下载并安装JDK 21
2. 配置环境变量`JAVA_HOME`指向JDK安装目录
3. 将`%JAVA_HOME%\bin`添加到`PATH`环境变量
4. 验证安装：`java -version`

#### 2. 安装MySQL

1. 下载并安装MySQL 5.7或更高版本
2. 启动MySQL服务
3. 创建数据库：`CREATE DATABASE unimall CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;`
4. 导入初始化SQL脚本：`mysql -u root -p unimall < sql/unimallv4.sql`

#### 3. 安装Redis

1. 下载并安装Redis 5.0或更高版本
2. 启动Redis服务：`redis-server`

#### 4. 安装Maven

1. 下载并解压Maven
2. 配置环境变量`MAVEN_HOME`指向Maven安装目录
3. 将`%MAVEN_HOME%\bin`添加到`PATH`环境变量
4. 验证安装：`mvn -version`

#### 5. 安装Node.js

1. 下载并安装Node.js 14或更高版本
2. 验证安装：`node -v` 和 `npm -v`
3. 安装cnpm（可选，加速依赖安装）：`npm install -g cnpm --registry=https://registry.npm.taobao.org`

### 后端部署

#### 1. 配置数据源

编辑`unimall-runner/src/main/resources/application.yaml`文件，修改以下配置：

```yaml
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/unimall?autoReconnect=true&useUnicode=true&characterEncoding=utf-8&allowMultiQueries=true
    username: root
    password: your_mysql_password
  redis:
    host: localhost:6379
  user-redis:
    host: localhost:6379
  lock-redis:
    host: localhost:6379
```

#### 2. 编译打包

在项目根目录执行命令：

```bash
mvn clean package -Dmaven.test.skip=true
```

编译完成后，生成的jar包位于`unimall-runner/target/unimall-runner-v4.jar`

#### 3. 启动后端服务

```bash
java -jar unimall-runner/target/unimall-runner-v4.jar
```

服务将在`http://localhost:8000/unimall`启动

### 前端部署

#### 1. 后台管理系统（unimall-admin）

1. 进入后台管理系统目录：`cd unimall-admin`
2. 安装依赖：`npm install` 或 `cnpm install`
3. 配置后端API地址：编辑`unimall-admin/config/dev.env.js`文件

```javascript
module.exports = {
  NODE_ENV: '"development"',
  HOST: '"http://localhost:8000"',
  BASE_API: '"http://localhost:8000/unimall/m.api"'
}
```

4. 启动开发服务器：`npm run dev`
5. 访问后台管理系统：`http://localhost:9528`

#### 2. 移动端应用（unimall-app）

**方式一：使用HBuilderX开发**

1. 下载并安装HBuilderX
2. 打开HBuilderX，选择"文件" -> "导入" -> "从本地目录导入"，选择`unimall-app`目录
3. 配置后端API地址：编辑`unimall-app/config/.env.development`文件

```javascript
module.exports = {
  baseUrl: 'http://localhost:8000/unimall'
}
```

4. 运行项目：点击HBuilderX工具栏上的"运行"按钮，选择对应的运行方式（浏览器、小程序、APP等）

**方式二：使用命令行开发**

1. 进入移动端应用目录：`cd unimall-app`
2. 安装依赖：`npm install` 或 `cnpm install`
3. 启动H5开发服务器：`npm run dev:h5`
4. 访问H5应用：`http://localhost:8080`

### 访问项目

- 后台管理系统：`http://localhost:9528`（默认账号：admin，密码：1234567）
- 移动端H5应用：`http://localhost:8080`
- 后端API：`http://localhost:8000/unimall`

### 常见问题

1. **端口冲突**：如果8000、9528或8080端口被占用，可以修改配置文件中的端口号
2. **数据库连接失败**：检查MySQL服务是否启动，用户名、密码和数据库名称是否正确
3. **Redis连接失败**：检查Redis服务是否启动，配置文件中的Redis地址是否正确
4. **前端编译失败**：尝试删除`node_modules`目录，重新安装依赖
