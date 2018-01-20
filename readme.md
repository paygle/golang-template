# go语言环境搭建-简单模板

## 安装

* 安装 go 环境 https://github.com/golang/go

* 配置 GOROOT 即 go 安装目录

* 配置 GOPATH 即工作目录此目录包含三个文件夹（bin，pkg, src），可以配置多个目录

* 解压下载的源码到 src 目录 运行根目录下的 packages-install.cmd文件

* 使用 go get -u github.com/golang/dep/cmd/dep 安装官方依赖管理工具dep

* 在 GOPATH/src 目录下创建自己的项目或 git 获取本项目即配置完成

* 在项目目录下执行 dep init 初始化依赖文件

* 在CMD中执行 go env 查看环境是否配置正确



## dep 帮助

```cmd
Usage: "dep [command]"

Commands:

  init     Set up a new Go project, or migrate an existing one
  status   Report the status of the project's dependencies
  ensure   Ensure a dependency is safely vendored in the project
  prune    Prune the vendor tree of unused packages
  version  Show the dep version information

Examples:
  dep init                               set up a new project
  dep ensure                             install the project's dependencies
  dep ensure -update                     update the locked versions of all dependencies
  dep ensure -add github.com/pkg/errors  add a dependency to the project
```