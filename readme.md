想自己写一个小工具实现简易的切换 npm 源

思路 1，调用命令 设置源
npm config set registry 源地址

思路 2 使用查看命令获取源地址
npm config get registry

##### 本地使用

npm install 如果你只是想在项目的本地环境中使用 mmp 命令，你可以通过以下命令安装项目的依赖项（包括 bin 脚本）：
安装完成后，你可以通过 npx 来运行你的 bin 脚本：npx mmp

比如 npx mmp list

##### mmp ls 查看目前源

- npm------- https://registry.npmjs.org/

  yarn------ https://registry.yarnpkg.com/

  tencent--- https://mirrors.cloud.tencent.com/npm/

  cnpm------ https://r.cnpmjs.org/

  taobao---- https://registry.npmmirror.com/

  npmMirror- https://skimdb.npmjs.com/registry/

##### mmp use 切换源

选择你要切换的源

##### mmp current 查看当前源

当前源: npm

##### mmp add 添加源

1.输入添加的名称 2.输入源地址

##### mmp ping 测试源

? 请选择镜像 cnpm
响应时长: 1635ms

##### mmp delete 删除自定义源

add 添加的源都可以删除

##### mmp rename 重命名

自定义添加的源都可以进行重新命名

##### mmp edit 编辑自定义镜像地址

# 用法 Usage

Usage: mmp [options] [command]

Options:

-V, --version output the version number

-h, --help display help for command

Commands:
ls 查看镜像

use 请选择镜像

current 查看当前源

ping 测试镜像地址速度

add 自定义镜像

delete 删除自定义的源

rename 重命名

edit 编辑自定义镜像地址

help [command] display help for command
