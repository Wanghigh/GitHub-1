# 第二周前端组任务


## git部分
 > 简介: Git是一个非常流行的版本管理软件, 多用于程序员团队项目协作. 基于git的GitHub是全球公认的最大开源社区, 许多著名的项目都是使用GitHub平台进行开发的, 后来也有GitLab等后起之秀, 强烈推荐大家都去注册一个GitHub账号, GitHub上有很多的项目能够开拓你们的视野, 激发你们的潜在的能力
- 首先安装Git, Windows用户: [点这里下载](https://git-scm.com/downloads), Linux用户: 我们有强大的软件包管理器, Mac OS用户: [点这里下载](https://git-scm.com/downloads)
### 注册一个码云Gitee账号
- 码云首页: [https://gitee.com/](https://gitee.com/)
#### 为什么不是GitHub?
- 去年的我们在接受培训的时候用的也是GitHub, 但是有一个问题一直存在: `速度太慢`.
- 从去年7月份开始使用 `码云Gitee` 之后, 经过漫长的使用到现在, 它的速度是很棒的(毕竟服务器在国内)
- 当然, GitHub更加国际化, 推荐大家都去注册一个, Gitee和GitHub我全都要.jpg
 ### 配置SSH公钥
 - Windows用户打开 `Git Bash`, Linux和Mac OS用户打开终端
 - 输入执行: `ssh-keygen -t rsa -C "your_email@youremail.com"`, 后面三次回车就行了
- 输入执行: `cat ~/.ssh/id_rsa.pub`, 下面会显示出已经生成好的公钥, 复制下来
- 通过主页右上角 「个人设置」->「安全设置」->「SSH公钥」->「添加公钥」, 添加生成的公钥添加到当前账户中
- 添加后, 在终端输入执行: `ssh -T git@gitee.com`, 若返回 `Hi 你的用户名! You've successfully authenticated, but Gitee.com does not provide shell access.`, 那么这一步就完成了
> 码云官方文档: [SSH 公钥设置](https://gitee.com/help/articles/4191), [生成/添加SSH公钥](https://gitee.com/help/articles/4181)(注意不要跟着上面的文档, 最后配置成仓库公钥了)
### 创建第一个仓库
 - 仓库名请根据各组的要求命名, 仓库类型是 `公开仓库` (运维组统一命名`Dev_ops`)
 - 码云官方文档: [创建你的第一个仓库](https://gitee.com/help/articles/4120)
### 将这个仓库clone到本地
- 在合适的位置创建一个文件夹, 专门放从码云仓库的, 比如命名叫做 `gitee`
 - 打开这个文件夹, 右键打开 `Git Bash`, Linux和 Mac OS右键在此处打开终端
 - 输入执行这两个命令: `git config --global user.name "your name"`, `git config --global user.email "your_email@youremail.com"`
- 再输入执行: `git clone https://gitee.com/用户个性地址/你的仓库名.git` (这个网址很好复制, 在仓库页面点击 `克隆/复制`, 一键复制HTTPS的那个就行)
- 下载完之后就会出现你的仓库了
### 将上周完成的网页工程文件提交到远程仓库
 - 打开刚刚克隆下来的整个仓库的文件夹
- 新建一个表示第一周的文件夹, 把工程文件放在这个文件夹
- 在最外面一级文件夹右键打开 `Git Bash` (就是能看到仓库里所有文件的地方, 也就是刚刚打开仓库文件夹的地方) 或者终端里面按顺序执行以下命令:
     - `git add .`
        - `git commit -m "first"`
        - `git push`
 - 这样就完成提交文件了, 为了方便大家少打两行命令, 可以把这三行命令写在一个脚本文件里面, 详见这个仓库最外面的的 **[点击查看 push.sh](./push.sh)**
*  那么问题来了: 远程仓库的代码更新了, 我怎么同步到本地?
>  一行 `git pull` 的事情而已

## 作业
* [美食美刻网页](https://pan.baidu.com/s/1djves8vV1L2RmMKobwgIDg)(提取码:dofg)

> 这个是.psd文件

* 像素大厨

>就是这个PxCook文件，可以下载下来。
>
>如果用不了，就点击一下（AdobeAIRInstaller.exe）这个应用程序，或者自己去重新下载一个，Adobe AIR文件也行的。

## 要求
> 1. 学会ps切图功能,或者学会使用pxcook
> 2. 熟练掌握css浮动定位的用法
> 3. 交作业时还是建立一个工程文件,文件的命名尽量规范,样式的书写也要规范如css类选择器命> 名最
> 好能查一下命名规范的文档
> 4. 写页面主要用div+css写页面布局,写html时注意不要随意嵌套标签,书写css样式尽量不要写内联> 样式,样式都写在css文件夹下面,选择器使用时注意看是否选中了页面元素
> 5. 复习上一周培训所学的内容,最好能把上一周的任务再快速的做一遍, 发给大家的视频尽量看, > 本
> 周的任务比上一周而言更加具有挑战性希望大家积极努力完成   
> 6. 本次作业要讲究整体布局,大家先把整体布局写完再写局部样式
> 7. 本周上交一个网页文件,另外还有每一周的周总结


