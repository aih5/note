
# 使用NPM安装
安装GitBook的最佳方法是通过NPM。在终端提示符下，只需运行以下命令即可安装GitBook：

```
$ npm install gitbook-cli -g
```

gitbook-cli是一个在同一系统上安装和使用多个版本的GitBook的实用程序。它将自动安装所需版本的GitBook来构建一本书。

创建一本书
GitBook可以设置样板书：
```
$ gitbook init
```

如果您希望将书籍创建到新目录中，可以通过运行来完成
```
gitbook init ./directory
```

使用以下方式预览和提供您的书
```
$ gitbook serve
```

或使用以下方法构建静态网站：
```
$ gitbook build
```

安装预发布版
gitbook-cli 可以轻松下载和安装其他版本的GitBook来测试你的书：
```
$ gitbook fetch beta
```

使用gitbook ls-remote列出可供安装远程版本。
调试
您可以使用这些选项--log=debug并--debug获得更好的错误消息（使用堆栈跟踪）。例如：
```
$ gitbook build ./ --log=debug --debug
```