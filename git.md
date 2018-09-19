# git使用
1. [下载git](https://git-scm.com/downloads)
2. 配置阿里镜像下载地址(以使用$ cnpm install [name]):
`npm install -g cnpm --registry=https://registry.npm.taobao.org`
3. 配置用户信息
``` 全局配置
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"
```
4. 基本命令
```
$ git remote add origin https://github.com/zlunr/note.git  **绑定提交地址**
$ git push -u origin master **使用绑定的远程地址提交**
$ mkdir my-dir-name **创建my-dir-name文件夹**
$ cd my-dir-name    **进入my-dir-name文件夹**
$ pwd       **显示完整路径**
$ cd ..     **返回上级目录**
$ ls        **当前目录列表**
$ git status    **查看仓库当前的状态**
$ git diff  **顾名思义就是查看difference**
$ git add ./    **将所有文件添加到仓库门口**
$ git commit -m '提交说明'  **将仓库门口的文件提交到仓库**
$ git log   **查看日志**
$ git log --pretty=oneline  **查看精简版日志**
$ git reflog    **用来记录你的每一次命令**
$ git reset --hard HEAD^ **返回上一个版本，上一个版本就是HEAD^，上上一个版本就是HEAD^^，当然往上100个版本写写成HEAD~100。）**
$ git reset --hard 1094a **跳到指定版本（1094a 为版本号）**
$ git checkout -- readme.txt    **撤销修改（回到最近一次git commit或git add时的状态）**
$ rm test.txt   **删除文件**
$ git clone git@github.com:michaelliao/gitskills.git    **克隆远程仓库**
```