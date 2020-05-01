#设置用户名和邮箱
git config --global user.name "myName"
git config --global user.email "myEmail"
#创建版本库
mkdir myRepository
cd myRepository
git init
#文件添加到仓库(可添加多个文件)、文件提交
git add readme.txt file2.txt
git commit -m "这是提示"

