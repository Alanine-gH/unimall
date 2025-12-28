# unimall-app 项目说明文档

## 1. 项目介绍

unimall-app 是一个基于 uni-app 框架开发的跨平台电商应用，支持 H5、微信小程序、支付宝小程序等多个平台。

## 2. 技术栈

- **框架**: uni-app (Vue 2)
- **构建工具**: Vue CLI 5.x
- **状态管理**: Vuex 3.x
- **HTTP 库**: flyio
- **开发工具**: HBuilderX

## 3. 开发环境要求

- **Node.js**: >= 14.0.0
- **npm**: >= 6.0.0
- **HBuilderX**: 最新稳定版

## 4. 克隆和安装步骤

### 4.1 克隆项目

```bash
git clone https://github.com/your-repository/unimall-app.git
cd unimall-app
```

### 4.2 安装依赖

**注意**: 项目存在依赖冲突问题，请使用以下命令安装依赖：

```bash
# 删除旧的依赖（如果存在）
rm -rf node_modules
rm package-lock.json

# 使用 --legacy-peer-deps 忽略依赖冲突
npm install --legacy-peer-deps
```

或者，您也可以修改 `package.json` 文件中的 eslint 相关依赖版本后再安装：

```json
{
  "devDependencies": {
    "eslint": "^7.32.0",
    "eslint-friendly-formatter": "^4.0.1",
    "eslint-loader": "^4.0.2",
    "eslint-plugin-vue": "^7.18.0",
    "babel-eslint": "^10.1.0"
  }
}
```

然后执行：

```bash
npm install
```

## 5. HBuilderX 配置

### 5.1 导入项目

1. 打开 HBuilderX
2. 点击 `文件` -> `导入` -> `从本地目录导入`
3. 选择项目所在目录，点击 `导入`

### 5.2 配置运行环境

1. 在 HBuilderX 中点击 `运行` -> `运行到浏览器` -> 选择您常用的浏览器
2. 或点击 `运行` -> `运行到小程序模拟器` -> 选择对应的小程序模拟器

## 6. 运行项目

### 6.1 使用 HBuilderX 运行

- **H5 端**: 点击 `运行` -> `运行到浏览器` -> 选择浏览器
- **微信小程序**: 点击 `运行` -> `运行到小程序模拟器` -> `微信开发者工具`
- **其他平台**: 类似上述步骤选择对应的平台

### 6.2 使用命令行运行

```bash
# 运行 H5 开发环境
npm run dev:h5

# 运行微信小程序开发环境
npm run dev:mp-weixin

# 构建 H5 生产版本
npm run build:h5

# 构建微信小程序生产版本
npm run build:mp-weixin
```

## 7. 注意事项

### 7.1 依赖冲突问题

项目使用了 Vue CLI 5.x (webpack 5.x)，但部分旧版本依赖（如 eslint-loader 2.0.0）只兼容 webpack 4.x。解决方法：

- 使用 `npm install --legacy-peer-deps` 安装依赖
- 或升级 eslint 相关依赖到兼容 webpack 5.x 的版本

### 7.2 微信小程序配置

- 确保已安装微信开发者工具
- 在微信开发者工具中开启 `服务端口`（设置 -> 安全设置 -> 服务端口）

### 7.3 API 接口配置

项目接口配置文件位于 `src/config/index.js`，可根据需要修改开发和生产环境的接口地址：

- 开发环境: `src/config/.env.dev.js`
- 生产环境: `src/config/.env.prod.js`

## 8. 项目结构说明

```
unimall-app/
├── src/                    # 源码目录
│   ├── components/         # 公共组件
│   ├── config/             # 配置文件
│   ├── filters/            # 过滤器
│   ├── pages/              # 页面
│   │   ├── address/        # 地址管理
│   │   ├── cart/           # 购物车
│   │   ├── category/       # 分类
│   │   ├── coupon/         # 优惠券
│   │   ├── index/          # 首页
│   │   ├── order/          # 订单
│   │   ├── pay/            # 支付
│   │   ├── product/        # 商品
│   │   ├── public/         # 公共页面
│   │   ├── set/            # 设置
│   │   └── user/           # 用户中心
│   ├── static/             # 静态资源
│   ├── store/              # Vuex 状态管理
│   ├── App.vue             # 根组件
│   ├── main.js             # 入口文件
│   ├── manifest.json       # uni-app 配置
│   └── pages.json          # 页面路由配置
├── .eslintignore           # ESLint 忽略配置
├── .eslintrc.js            # ESLint 配置
├── babel.config.js         # Babel 配置
├── package.json            # 项目依赖
├── postcss.config.js       # PostCSS 配置
└── README.md               # 项目说明
```

## 9. 常见问题及解决方案

### 9.1 安装依赖失败

**问题**: 执行 `npm install` 时出现依赖冲突错误
**解决**: 使用 `npm install --legacy-peer-deps` 或升级冲突的依赖版本

### 9.2 运行到微信小程序失败

**问题**: 无法连接到微信开发者工具
**解决**:

1. 确保微信开发者工具已安装
2. 在微信开发者工具中开启服务端口
3. 检查 HBuilderX 中的微信小程序配置是否正确

### 9.3 API 接口调用失败

**问题**: 无法调用后端 API 接口
**解决**:

1. 检查 `src/config/index.js` 中的接口地址配置
2. 确保后端服务已启动
3. 检查网络连接是否正常

## 10. 联系方式

如有问题，请联系项目维护人员：

- 邮箱: kongshuo2006@163.com
- 微信: k872554633

---

**注意**: 本项目仅供学习和开发使用，请勿用于商业用途。
