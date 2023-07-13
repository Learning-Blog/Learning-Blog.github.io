## 1. 什么是nvm？
> Node.js 默认一台电脑只能装一个版本，有时为了开发项目经常会使用不同版本的Node.js 版本，通常情况版本切换就比较麻烦了。
为了解决这个问题，**nvm** （node version manager）应运而生。有了 **nvm**，便可以在一台电脑上安装多个 Node.js 版本，并且可以一条指令随时下载或切换版本，而不需要频繁地下载/卸载不同版本的 node.js 来满足当前项目的要求。

## 2. 安装nvm
> **github下载地址：** https://github.com/coreybutler/nvm-windows/releases
> - **nvm-noinstall.zip：** 绿色免安装版本，但是使用之前需要配置
> - **nvm-setup.zip：**安装版，下载之后点击安装，无需配置就可以使用

## 3. 常见命令

>1. **nvm -v //查看nvm版本**
> - nvm --version ：显示 nvm 版本


>2. **nvm list  //显示版本列表**
> - nvm list ：显示已安装的版本（同 nvm list installed
> - nvm list installed：显示已安装的版本
> - nvm list available：显示所有可以下载的版本


>3. **nvm install  //安装指定版本node.js**
> - nvm install 14.5.0：安装 14.5.0 版本的 node.js
> - nvm install latest：安装最新版本


>4. **nvm use //使用指定版本node**
> - nvm use 14.5.0： 切换到 14.5.0 版本的 node.js
> - --lts // 自动切换到长期支持版本
> - --lts=<LTS name> // 自动切换到指定名称的node长期支持版本


>5. **nvm uninstall <version> //卸载指定版本 node**
> - nvm uninstall 14.5.0：卸载到 14.5.0 版本的 node.js
> - nvm uninstall --lts // 卸载长期支持版本的node
> - nvm uninstall --lts=<LTS name> // 卸载一个指定名称的长期支持版本的node

> 6.**nvm --help //显示命令行帮助信息**
> - [ ps：在运行nvm install 的时候，有可能会出现无权限安装的问题，请 以管理员身份运行 cmd ]

## 4. 其他命令
> nvm deactivate // 取消当前nvm命令行效果

> 1. **nvm 查看node版本**
> - nvm current // 查看当前使用的node版本
> - nvm ls // 查看所有本地可用的node版本
> - nvm ls <version> // 参看指定版本
> - nvm ls-remote // 查看所有可用远程版本
> -  --lts // 查看所有长期支持版本
> - nvm ls-remote <version> // 参看所有node的指定远程版本
> - --lts // 查看所有node长期支持版本
> - --lts=<LTS name> // 仅查看指定名称的长期支持版本

> 2. **nvm 版本别名**
> - nvm alias [<pattern>] // 显示所有以<pattern>开头的版本别名
> - nvm alias <name> <version> // 给版本<version>设置一个别名
> - nvm unalias <name> // 删除<name>的版本别名

> 3. **nvm和npm**
> - nvm **install**-latest-npm // 在当前node版本中，将npm升级到最新版
> - nvm **reinstall**-packages <version> // 在全局重新安装npm，从<version>版本到当前版本

> 4. **npm which显示安装路径**
> - npm **which** [current | <version>] //显示已安装node的安装路径。

> 5. **nvm缓存**
> - nvm **cache** dir // 显示nvm的缓存目录
> - nvm **cache** clear // 清楚nvm的缓存目录

> **6. nvm运行node**
> - nvm **exec** [--silent] [version] [<command>] **// 在<version>运行命令<command> **
> - **nvm exec 4.8.3 node app.js** //Run `node app.js` with the PATH pointing to node 4.8.3
> - nvm **run** [--silent] [version] [<args>] **// 在<version>以参数<args>运行node --**
> - **nvm run 6.10.3 app.js** //Run app.js using node 6.10.3

> - `nvm on` ：开启node.js版本管理。
> - `nvm off` ：关闭node.js版本管理。

> - `nvm node_mirror [url] `：设置node镜像。默认是https://nodejs.org/dist/。
> - 如果不写url，则使用默认url。设置后可至安装目录settings.txt文件查看，也可直接在该文件操作。
> - `nvm npm_mirror [url] `：设置npm镜像。https://github.com/npm/cli/archive/。
> - 如果不写url，则使用默认url。设置后可至安装目录settings.txt文件查看，也可直接在该文件操作。

