#设置用户名和邮箱
git config --global user.name "myName"
git config --global user.email "myEmail"

#创建版本库
mkdir myRepository
cd myRepository
git init

#文件添加暂存区（stage）
git add readme.txt
#文件提交到 (master)
git commit -m  "这是提示"


#打印最近提交历史
git log
#记录提交和重置的命令，最前面是版本id
git reflog
#查看状态
git status


#回退到某个版本，HEAD^表示上个版本 ,HEAD^^表示上上个版本。 
git reset --hard HEAD^
git reset --hard 版本id


#三种回退场景
#场景1.文件保存但没有添加到暂存区，恢复
git restore file
#场景2.文件添加到暂存区，但没有提交，恢复到场景1
git restore --staged file
#场景3.文件已提交，但未发布到远程仓库，使用版本回退

