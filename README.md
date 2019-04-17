1、 环境安装
Git最新版下载地址：https://gitforwindows.org/
git和TortoiseGit都需要单独安装
TortoiseGit，Git客户端，32/64位最新版及对应的语言包下载地址：https://tortoisegit.org/download/
[图片]

先安装git 再安装TortoiseGit ，再安装语言包
2、配置
[图片]

[图片]
本地项目配置文件 “Edit local .git/config” 
“Edit global .git/config”按钮，会使用记事本打开全局配置文件
[图片]

3、密钥
a、git密钥（TortoiseGit 不需要配置，这是git自带Git GUI需要设置的）
[图片]

[图片]
选择show SSH Key
[图片]
将上诉密钥导入到远程仓库ssh key


b、客户端密钥
安装目录bin下（如D:\Program Files\TortoiseGit\bin） 找到 puttygen.exe
[图片]
双击打开
[图片]

注意参数，Parameters，Type of key to generate 
要选择第三个或者第四个：（ECDSA、ED25519），点击Generate生产密钥，要不断移动鼠标
[图片]
保存公私钥在本地，以便以后使用
将公钥导入到远程仓库ssh key
4、克隆一个项目
空白处右键，选择: Git clone
[图片]
输入远程gitlab地址
本地保存地址
[图片]
点击OK
[图片]
点击show log
[图片]


Git Pull是从远端拉取最新的代码
Git Fetch是从远端拉取最新的分支
Git Push是将本地仓库的代码提交到远端
Git Commit ->”master”，将本地代码提交到本地版本库（默认的分支是master）。
5、将本地代码提交到本地仓库
新建一个文件Git 2.21.0&TortoiseGit 2.8.0.0，里面有git客户端相关的文件
右键
[图片]
在文件夹里面选择Git Commit ->”master”
填写提交备注message（不填写不允许提交），勾选需要提交的文件，点击commit，即可将本地代码提交到本地版本库
[图片]
点击提交
[图片]
6、将本地文件推送到远端仓库
右键空白处，选择Git Push，出现如下弹框：
[图片]

选择本地、远端版本库
点击远端 manage 配置远端地址（如远端无该项目，需新增项目）
[图片]

[图片]
点击ok
[图片]

[图片]
查看远端仓库
[图片]
