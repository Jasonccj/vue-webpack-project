# 个人小记   
## 1.package.json文件中devDependencies与dependencies   
devDependencies  里面的插件只用于开发环境，不用于生产环境。  
dependencies  是需要发布到生产环境的。    
像使用的一些构建工具比如glup、webpack这些只是在开发中使用的包，上线以后就和他们没关系了，所以将它写入devDependencies。  
## 2.package.json dependencies版本符号   
指定版本：比如1.2.2，遵循“大版本.次要版本.小版本”的格式规定，安装时只安装指定版本。   
波浪号（tilde）+指定版本：比如~1.2.2，表示安装1.2.x的最新版本（不低于1.2.2），但是不安装1.3.x，也就是说安装时不改变大版本号和次要版本号。   
插入号（caret）+指定版本：比如ˆ1.2.2，表示安装1.x.x的最新版本（不低于1.2.2），但是不安装2.x.x，也就是说安装时不改变大版本号。需要注意的是，如果大版本号为0，则插入号的行为与波浪号相同，这是因为此时处于开发阶段，即使是次要版本号变动，也可能带来程序的不兼容。   
latest：安装最新版本。   

## 3.webpack-dev-server --inline --progress --config   
--inline 具体还有一个iframe，他们的最后效果都是一样的，都是监听文件变化，然后在将编译后的文件推送到前端完成页面的reload的。   
--progress 显示打包进度   
[参考文档](https://segmentfault.com/a/1190000006670084)   
