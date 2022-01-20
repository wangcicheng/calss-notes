# 寒假学习笔记
## 1.19
### 学习内容
- 重新看了一遍视频，下载了 [nodejs](https://nodejs.org/en/)、[nginx](https://nginx.org/en/download.html)、[vs code](https://code.visualstudio.com/)、[git](https://git-scm.com/downloads) 等开发工具
- 对自己新建的本地静态页面目录进行了访问
- nodejs 显示+打印时间
- 使用npm包管理工具进行初始化（init）、下载（install）dayjs包并进行使用
```
 console.log("hello world!")

 const date = new Date();
 console.log(date.getTime());
```
- use dayjs package  result(2022-01-19 10:06:06)
```
 const dayjs = require("dayjs")
 console.log(dayjs().format('YYYY-MM-DD hh:mm:ss'));
```

### 一些小注意事项
- 执行 nginx 时命令行输入时应为 nginx.exe
- nodejs 中 console.log("hello world")是没有分号的，可写可不写
- npm(node package manage) 下载node自带的包管理工具 

## 1.20
### 学习内容
- git工具的使用

    1、三个概念：工作区、暂存区、仓库

    - `git add` 工作区到暂存区
    - `git commit` 暂存区到仓库
    - `git status` 查看文件状态
    - `git clone` 从远程仓库下载
    - `git push` 推送到远程仓库

    2、文件状态 `git status`
    - `Changes not staged for commit`

        工作区中有改内容，但是暂存区没有，我们需要通过 `git add` 将其添加进暂存区

    - `Changes to be committed`

        已经被添加进暂存区的文件，可以通过 `git commit` 提交到版本库，也可以使用 `git reset HEAD <file>` 来撤销暂存
`
    - `Untracked files`

        未追踪的文件，可以通过 `git add` 添加进暂存区

    - `nothing to commit, working tree clean`

        工作区所有的更改都已经提交至版本库


