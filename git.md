
dir: .git
# config
- 配置信息
# .git/refs 引用
- /tags 里程碑
- /heads 分支，独立的开发空间，比如前端和后端
    - master 
        - git cat-file -t ，t为类型
        - commit 类型，指针指向的commit
        - 看类型用t，看内容用p
    - branch
    - git checkout 与HEAD一样

# commit tree blob 三个对象之间的关系
- **blob** 具体文件
- **tree** 具体文件夹
- **commit** 某一个时刻的快照,项目包含的东西
# detached HEAD
 - 替换头指针之后，需要将其与某个分支绑定，以避免于被git丢弃掉# detached HEAD
 - 按照git提示创建新的分支
 - HEAD 一般指向分支最后一次 提交的commit
 - HEAD 处于分离头指针时，其可能指向某一个具体的commit，没有对应的分支
 - 分支切换后，HEAD 也会跟着切换

# 清除分支
- git branch -d 分支名
- git branch -D 分支名
<<<<<<< HEAD

# 修改最近一次commit的message
- git commit --amend -1

# 历史记录
- git rebase -i 
- [git rebase 用法](https://www.jianshu.com/p/4a8f4af4e803)
=======
>>>>>>> 39cbc095e4349cab12c2929e619d95064ac6dc89

# git diff --cached
比较暂存区和HEAD 的差异

# 工作区和暂存区的比较
### 比较所有
- git diff
### 比较一个或者多个文件变更
- git diff --readme

### 不保暂存区去的所有文件
- git reset HEAD
### 让工作区的文件恢复为暂存区，和暂存区一
- git checkout -- <file name > # 丢弃工作区内容，恢复到暂存区
- git reset HEAD  #变更为暂存区的内容
#### 恢复部分暂存区文件到工作区
- git reset HEAD -- <file name>
#### git reset --hard <commit>
