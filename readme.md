<!-- encoding: UTF-8 -->
#纳米光子学实验室 @SEU电子学院
## 主页维护
### 维护
直接编辑HTML并推送
### 部署
- 仓库托管于https://github.com/shuoxinma4/SEU_QUANTUM_NANOPHOTONICS_LABORATORY
- 网页托管于cloudflare，shuoxinma账号
### 新建
- 注册github,注册cloudflare
- 查看cloudflare教程 https://developers.cloudflare.com/pages/tutorials/forms/#live-example
- - Key point 1: 应添加默认index.html
- - Key point 1: 将网页放在子目录(public)，并设置Build settings->Build output directory: /public
- 新建git仓库，注意编码为UTF-8，推送github并设置public
- 在cloudflare中，Account home-> Create application -> Pages -> import...Git
- 选择主分支。每次推送主分支后，cloudflare将自动抓取、构筑并发布
### 从已有SEU网页更新
- 不要直接另存为：Edge会自动修正源码中链接地址
- 安装GNU wget下载工具
- - https://eternallybored.org/misc/wget/
- 下载现有网页，参考指令(会自动下载被链接页面)
- - wget --mirror --convert-links --page-requisites --no-parent --adjust-extension --no-host-directories https://electronic.seu.edu.cn/_upload/tpl/0b/93/2963/template2963/research.htm

