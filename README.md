# 测试练习使用git+github
## 1.建立本地仓库
**git init：使得本地文件夹变成一个仓库**

## 2.添加修改后的文件到暂存区
**git add . ：**添加所有文件到暂存区

**git add xxx.html：**添加xxx.html到暂存区

## 3.将暂存区的文件提交到本地仓库
**git commit -m " 添加xxx.html文件，文件中添加一个div "**

## 4.将本地仓库的项目上传至远程仓库
### (1)使用SSH传输；首先生成SSH密钥：
```Linux
ssh-keygen -t rsa -C "邮箱"
```

​    生成的密钥存储在"C:\Users\.ssh\id_rsa.pub"
### (2)打开github->setting->SSH and GPG keys
将id_rsa.pub的内容粘贴到此

### (3)添加远程仓库地址(TestGit是自己起的别名)
    git remote add TestGit https://github.com/WriteCodee/Test.git
### (4)将本地仓库的文件上传到远程仓库
    git push -u TestGit master