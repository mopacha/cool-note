# 基于VUE-SSR 的工程化实践

Node.js Web框架，基于 Koa2

## 前言

> - CSR: client-side-render
> - SSR: server-side-render，服务端渲染，这里理解为同构应用


后端渲染、客户端渲染(CSR)、同构应用(SSR)

> - 后端渲染：服务器直接生成HTML文档并返回给浏览器，但页面交互能力有限。适用于任何后端语言：PHP、Java、Python、GO等。
> - 客户端渲染：页面初始加载的HTML文档中无内容，需要下载执行JS文件，由浏览器动态生成页面，并通过JS进行页面交互事件与状态管理。
> - 同构：isomorphic/universal，基于react、vue框架，客户端渲染和服务器端渲染的结合，在服务器端执行一次，用于实现服务器端渲染（首屏直出），在客户端再执行一次，用于接管页面交互，

核心解决SEO和首屏渲染慢的问题。


## 技术栈

- Nodejs、Koa2
- vue、vue-router、vuex
- ElementUI
- webpack4
- axios
- babel7、eslint
- css、scss、postcss
- pm2
- log4js




## 开始使用

1. 安装 node/npm  Node: >=8
2. clone 模板项目
	```
	git clone https://github.com/mopacha/vue-ssr-admin.git
	```

3. 启动

	```
	npm install
	npm start 
	```
	
 ## 目录结构


## 部署 

1. 安装 node/npm  Node: >=8
2. 安装pm2
   
	```bash
	npm i -g pm2 
	```
3. 安装pm2-intercom;

	```bash
	pm2 install pm2-intercom
	```

4. 构建生产代码
	```bash
	npm run build
	```
5. pm2启动服务
	```npm
	pm2 start pm2.config.js --env production
	```











