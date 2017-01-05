#### CDN

推荐：unpkg, 会保持和 npm 发布的最新的版本一致。可以在 unpkg.com/vue/ 浏览 npm 包资源。
也可以从 jsdelivr 或 cdnjs 获取，不过这两个服务版本更新可能略滞后。
<script src="https://unpkg.com/vue/dist/vue.js"></script>

#### NPM
在用 Vue.js 构建大型应用时推荐使用 NPM 安装， NPM 能很好地和诸如 Webpack 或 Browserify 模块打包器配合使用。 Vue.js 也提供配套工具来开发单文件组件。

#### 最新稳定版
$ npm install vue


#### 开发版本

重要: Github 仓库的 /dist 文件夹只有在新版本发布时才会更新。如果想要使用 Github 上 Vue 最新的源码，你需要自己构建。
git clone https://github.com/vuejs/vue.git node_modules/vue
cd node_modules/vue
npm install
npm run build
Bower

#### 最新稳定版本
$ bower install vue

#### 命令行工具

Vue.js 提供一个官方命令行工具，可用于快速搭建大型单页应用。该工具提供开箱即用的构建工具配置，带来现代化的前端开发流程。只需几分钟即可创建并启动一个带热重载、保存时静态检查以及可用于生产环境的构建配置的项目：
'''
	# 全局安装 vue-cli
	$ npm install --global vue-cli
	# 创建一个基于 webpack 模板的新项目
	$ vue init webpack my-project
	# 安装依赖，走你
	$ cd my-project
	$ npm install
	$ npm run dev
'''