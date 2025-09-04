[GitHub官网](github.com)  
# 一. 什么是GitHub
## 🛠核心概念
- 代码托管平台：基于 Git 版本控制系统，帮助开发者存储、管理和追踪代码的历史版本。

- 协作开发：支持多人同时参与同一个项目，方便团队分工、合并代码和解决冲突。

- 开源与私有仓库：既可以公开分享代码（开源），也可以建立私有仓库保护项目隐私。

## 📦 主要功能
- 版本控制：记录每一次代码修改，随时回溯历史版本。

- Pull Request（PR）：提交代码修改建议，方便团队审查和讨论。

- Issues：用于跟踪 bug、功能需求或任务。

- GitHub Pages：直接用仓库托管静态网站或博客。

- Gist：分享代码片段或文档的小工具。

- 社交功能：关注（Follow）、收藏（Star）、派生（Fork）项目，形成开发者社区。

## 🌍 发展与现状
- 成立时间：2008 年，由 Tom Preston-Werner、Chris Wanstrath 等人创立。      

- 收购：2018 年被微软以 75 亿美元收购。

- 用户规模：截至 2023 年，已有超过 1 亿开发者和数亿个代码仓库。

- 影响力：是全球最大的开源社区和代码托管平台之一。

# 二. 注册账户
首先是在官网上注册自己的GitHub账号。 注册完成后进行简单的设置，开始创建一个属于自己的库。

# 三. 创建仓库
（注意：由于我们是免费用户，因此只能创建公共仓库）

创建一个新仓库（点击右上角头像旁的"+"，选择"New repository"）

![创建新仓库](https://raw.githubusercontent.com/moiunaochen/github-beginners-guide/refs/heads/main/assets/1.png)

（1）"Repository name"是为自己的库起一个库名 

（2）"Description"是对自己的库进行一个简单的描述 

（3）选择仓库权限为"Public"，即建立公共存储库 

（4）可以选择"Initialize this repository with a README" 

（5）点击"Create repository"，创建存储库 

另外： gitignore: 不需要进行版本管理的仓库类型，对应生成文件.gitignore license: 证书类型，对应生成文件LICENSE

<img width="1362" height="1277" alt="image" src="https://github.com/user-attachments/assets/79804d64-966d-45eb-9914-987b0d489a79" />    

# 四. 什么是Git

Git 是一种分布式版本控制系统，最初由 Linux 之父 林纳斯·托瓦兹（Linus Torvalds） 在 2005 年创建，用来高效管理 Linux 内核的开发。它现在已经成为全球最流行的代码版本管理工具之一，也是 GitHub、GitLab 等平台的底层核心。

## 🛠 核心作用
- 版本控制：记录文件（尤其是代码）在不同时间的修改历史，可以随时回溯到任意版本。

- 多人协作：支持多人同时开发同一项目，并能合并不同人的修改。

- 分支管理：可以创建、切换、合并分支，让不同功能的开发互不干扰。

- 离线工作：因为是分布式，每个人的电脑上都有完整的版本库，即使没联网也能提交、查看历史。

你可以把它理解为，游戏存档。

# 五. 安装Git
进入[Git下载界面](https://git-scm.com/downloads)  以Windows为例

<img width="974" height="450" alt="image" src="https://github.com/user-attachments/assets/da757ae7-258a-4e05-9cc4-198f423f09d1" />

下载后双击运行，直接安装，在安装过程中直接默认选项即可。

检查Git是否安装成功，输入 `git --version`

<img width="600" height="323" alt="image" src="https://github.com/user-attachments/assets/93867004-4c78-4a50-bcef-f959819ed78b" />  

# 六. 配置Git  
以VS Code为例  

进入[VS Code下载界面](https://code.visualstudio.com/)

<img width="1321" height="757" alt="image" src="https://github.com/user-attachments/assets/0b8b026e-84c8-451e-8939-05c9ef2f09a3" />

下载后双击运行，直接安装，在安装过程中直接默认选项即可。

在VS Code中创建一个项目，项目文件夹下创建一个示例文件，用于测试。

<img width="1130" height="502" alt="image" src="https://github.com/user-attachments/assets/98db981a-f18c-44d6-beb2-8981b888ff75" />  

然后点击初始化仓库。

<img width="1504" height="785" alt="image" src="https://github.com/user-attachments/assets/1265a8a2-0302-4c06-b1b0-2d8ac232e0f3" />  

点击提交存档。

<img width="1545" height="748" alt="image" src="https://github.com/user-attachments/assets/b7b69c02-4cdd-4787-9443-7778a7e5ed56" />  

点击总是。

<img width="455" height="146" alt="image" src="https://github.com/user-attachments/assets/0d9fd249-8113-4311-a0a6-b5626add9142" />  

然后会提示设置 用户名 和 邮箱。

<img width="443" height="119" alt="image" src="https://github.com/user-attachments/assets/22bb504b-0abf-4abd-a84f-23c742d7fa8c" />  

（一般不用看）[Git名称邮箱详细配置教程](https://git-scm.com/book/zh/v2/%e8%b5%b7%e6%ad%a5-%e5%88%9d%e6%ac%a1%e8%bf%90%e8%a1%8c-Git-%e5%89%8d%e7%9a%84%e9%85%8d%e7%bd%ae)    

`git config --global user.name "John Doe"`  

`git config --global user.email johndoe@example.com`  

在终端输入以上两条命令（名字 和 邮箱 要替换为自己 GitHub的名称邮箱）

<img width="890" height="543" alt="image" src="https://github.com/user-attachments/assets/8037bba9-5cdc-4001-8d2e-5b659c7f6242" />  

然后就可以查看历史更新记录了

<img width="1286" height="638" alt="image" src="https://github.com/user-attachments/assets/98c207c1-6e14-4d2d-acc0-9072b591e652" />    
 
接下来将项目发布到GitHub会跳转到浏览器授权，直接同意就行

<img width="781" height="582" alt="image" src="https://github.com/user-attachments/assets/ffb01567-4bd5-4e24-ab24-20dbaf21e66b" />  

<img width="640" height="489" alt="image" src="https://github.com/user-attachments/assets/8157903e-efd7-49ac-8175-9b8c31276bab" />  

然后会出现两个选项，公开和私有，选择公开

<img width="951" height="444" alt="image" src="https://github.com/user-attachments/assets/0e9de157-3a37-404e-8cf9-24aa725a31ef" />      

一般情况这里会上传失败，因为没有设置 代理

<img width="652" height="210" alt="image" src="https://github.com/user-attachments/assets/972dc3be-b7ae-4211-bb13-fad0241e0439" />

<img width="654" height="250" alt="image" src="https://github.com/user-attachments/assets/f0c6c2a6-0024-4327-a248-8fe87bb97ceb" />  

[详细代理教程](https://stackoverflow.com/questions/783811/getting-git-to-work-with-a-proxy-server-fails-with-request-timed-out)

将下面的信息改成自己的

`git config --global http.proxy http://proxyuser:proxypwd@proxy.server.com:8080`  

`git config --global http.proxy http://127.0.0.1:7897`  

`git config --global https.proxy https://127.0.0.1:7897`    

点击提交，就可以发现提交成功了。

<img width="1513" height="902" alt="image" src="https://github.com/user-attachments/assets/716d83af-174d-4972-915c-2e01d565eb3e" />

暂时到此结束