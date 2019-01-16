#  vue-admin-template 手把手从零搭建全过程
## 1.基础搭建
新建README.md和.gitignore   
npm init 初始化  
npm i --save-dev webpack@4.16.5                                 安装webpack4   
npm i vue@2.5.17                                                安装vue   
npm i --save-dev vue-loader@15.3.0                              安装处理vue的vue-loader   

新建src文件夹,创建App.vue,创建build下的webpack.dev.conf.js文件并编写他们
npm i --save-dev webpack-dev-server@3.1.14                      安装webpack-dev-server   
npm i --save-dev css-loader@1.0.0                               安装webpack-dev-server依赖的css-loader   
npm i --save-dev html-webpack-plugin@4.0.0-alpha                安装html-webpack-plugin  

开始配置webpack.dev.conf.js文件
创建一个development和production的公有webpack配置文件webpack.base.conf.js