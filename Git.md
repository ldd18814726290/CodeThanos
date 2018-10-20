#Git
## 概念  Linux内核
    1.定义：分布式版本控制系统。
        Ⅰ.主支：master
        Ⅱ.分支：branch
    2.原理：
        [1] clone  克隆远程版本库,到本地版本库  代码和版本信息
        [2] branch 创建分支,修改代码
        [3] push   提交代码
        [4] merge  合并分支  【本地版本库】
        [5] fetch  取出代码  【远程版本库】
        [6] patch  生成补丁   
        [7] pull   上传代码   
    3.冲突：如果两者Developer代码冲突,一方解决,然后提交。
## 脚本命令
    创建版本库 init    mkdir—cd—init
    增加内容   add     
    提交内容   commit  
    管理分支   branch  
    
    版本回滚   revert
    [1]本地代码库   revert commit-id  回滚至某commit版本
    [2]远程代码库   第一步：回滚至某commit版本-本地分支
                  第二步：删除远程分支
                  第三步：重新提交本地分支
              
## GitHub
    1.GitHub:注册账号、创建repository
    2.Git:   设置用户名、邮箱
    3.IDEA:  [1] 设置Git                Path
             [2] 设置GitHub             Host、Token
             [3] 创建本地仓库 create     Reposity
             [4] 上传项目到本地仓库 add   暂存区  绿色
                                commit 版本库  白色
             [5] 上传项目到GitHub share  仓库名、描述    (、message)
             [6] 提交修改到GitHub add    暂存区  红色-新增文件
                                              蓝色-修改文件
                                commit 
                                push   GitHub    
                     