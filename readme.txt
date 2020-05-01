#设置用户名和邮箱
git config --global user.name "myName"
git config --global user.email "myEmail"

#创建版本库
mkdir myRepository
cd myRepository
git init

#文件添加到仓库(可添加多个文件)、文件提交
git add readme.txt 
git commit -m  "这是提示"

#打印最近3次提交历史
git log

#记录提交和重置的命令，最前面是版本id
git reflog

#回退到某个版本，HEAD^表示上个版本 ,HEAD^^表示上上个版本。 
git reset --hard HEAD^
git reset --hard 版本id



