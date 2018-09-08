安装
nvm 的官方版本只支持 Linux 和 Mac。 

安装只需执行

wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.29.0/install.sh | bash
或

curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.29.0/install.sh | bash

如果是 Windows 用户，可以用 nvm-windows 。 可能会有一些坑（我的 Win7 能比较正常的运行，而我一同事的，总出现问题。。。）。



常用命令

nvm install [Nodejs 版本] 安装某版本的Nodejs

nvm use [Nodejs 版本|system] 使用某版本的Nodejs。

若选的 system 表示用 电脑上在装 nvm 之前使用装的 Nodejs
nvm ls 查看本机安装的所有的 Nodejs, 并高亮当前使用的版本
当上面命令中的 Nodejs 版本缺省时，会在当前以及其上级文件夹中找 .nvmrc 文件，从该文件中读取 Nodejs 的版本值。



node 淘宝镜像
Ubuntu .bashrc 文件加上：export NVM_NODEJS_ORG_MIRROR=https://npm.taobao.org/mirrors/node

npm 淘宝镜像

npm install -g cnpm --registry=https://registry.npm.taobao.org

不同版本 node 的 npm 需要分别设置淘宝镜像
