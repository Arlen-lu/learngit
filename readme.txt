cd D:/MyGit   定位到git库地址
pwd  查询当前路径
mkdir projectname  新建文件夹
cd projectname 定位到项目文件夹
git init    在当前路径下创建并初始化Git 仓库，存放该项目的所有数据
必须先将git add到暂存区，才能git commit到版本库中去
git add filename  提交新增/修改的文件到暂存区
git commit -m "explanation about what you add"  将刚添加/修改的文件从暂存区提交到分支库，并且清空暂存区
git status   查看仓库当前状态，如文件被修改等
git diff  显示文件修改的具体内容
git log  查看修改记录
cat filename  查看文件内容
git reflog 查看每次执行的命令
git checkout -- filename    让文件回到最近一次git commit或git add时的状态。
git reset HEAD filename    把暂存区的修改回退到工作区
回退版本：  
git reset --hard HEAD^   回退到上一个版本
git reset --hard HEAD~100 会退到上100个版本
git reset --hard commit_id       回退/返回到对应版本(be68为commit id)
rm filename  删除工作区的文件
git rm filename 删除版本库中的文件
git checkout -- filename 使用版本库中的版本替换工作区的版本，即将版本库中的文件恢复到工作区中
MyGit 工作区
.git为版本库

ssh-keygen -t rsa -C "email"   创建SSH可以
git remote add origin git@github.com:username/filename.git   将本地库关联到github的库相关联
git push -u origin master             将本地库的所有内容推送到远程库上去，首次指定默认服务器，需要添加-u
ssh -T git@github.com                                          git链接github
git clone git@github.com:username/projectname克隆远程库到本地库中
ls 查看当前路径下的文件夹



新建分支，并切换到分支
将工作区修改的内容更新到分支中区，此时master分支内容保持不变
在dev库更新完成，并确认无误后，切换到master分支，并合并dev分支，此时两者库会变成同步的状态
分支管理
git checkout -b dev    创建名为dev的分支(-b表示创建并切换)
= git branch dev  +  git checkout dev   创建分支dev + 切换分支

git branch 查看当前分支
git checkout master  切换为master分支，切换分支前确保已将工作区内容更新到git库中去
git log 显示 End时，输入CTRL+C or “：q”
git merge  --no-ff -m “explanation”  dev  
将指定的dev分支合并到当前分支(即master分支)中去，内容完成同步
git branch -d dev 删除dev分支
git branch -D dev 强行删除dev分支
git log --graph   可查看分支合并图
branch test1 and test2
git stash 将当前工作现场“储藏起来”，后续恢复再继续，一般用在临时新建分支去解bug
git stash list 查看储存的工作现场
git stash pop = git stash apply + git stash drop 恢复并删除stash
git stash apply stash@{0} 选择指定的stash恢复