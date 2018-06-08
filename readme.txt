cd D:/MyGit   定位到git库地址
pwd  查询当前路径
mkdir projectname  新建文件夹
cd projectname 定位到项目文件夹
git init    在当前路径下创建并初始化Git 仓库，存放该项目的所有数据
git add filename  提交新增/修改的文件到暂存区
git commit -m "explanation about what you add"  将刚添加/修改的文件从暂存区提交到分支库，并且清空暂存区
git status   查看仓库当前状态，如文件被修改等
git diff  显示文件修改的具体内容
add log  查看修改记录
cat filename  查看文件内容
git reflog 查看每次执行的命令

回退版本：
git reset --hard HEAD^   回退到上一个版本
git reset --hard HEAD~100 会退到上100个版本
git reset --hard commit_id       回退/返回到对应版本(be68为commit id)

MyGit 工作区
.git为版本库