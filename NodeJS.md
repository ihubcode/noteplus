# Nodejs篇

[返回主目录](README.md)

> 
>
> 记录Nodejs使用过程中的一些实践心得

### 一、Nodejs版本管理



#### NVM 切换nodejs版本

[nvm](http://nvm.sh) 工具  下载地址：http://nvm.sh



- 首先，根据不同操作系统下载安装对应的nvm版本
- 其次，根据项目实际需要，在shell命令工具中使用`nvm install`  命令，安装N个不同版本的nodejs

```
$ nvm install <version> [arch]
```

举例：

```
// install v6
$ nvm install 6

// install v7
$ nvm install 7

// install latest
$ nvm install latest

//... install more version
```

- 最后，在系统本地安装一个nodejs版本（推荐最新版）
-  于是我们可以愉快的nvm切换玩耍了....

> 注释：windows下（其他系统下没有测试），安装nvm前系统不能存在nodejs版本的安装，否则当nvm切换nodejs版本后，npm将提示为无效命令

```
// 显示通过nvm已经安装好的nodejs版本列表
$ nvm list

// 切换nodejs版本
$ nvm use <version>

// 查看当前环境nodejs版本
$ node -v

// npm 命令...
$ npm -v 
$ npm intall pkgname [--save-dev]/[--save]
```

