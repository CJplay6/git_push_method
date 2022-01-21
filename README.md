# git_push_method

## 建立本地和仓库的关联

1. git init

2. git remote add origin ssh路径 (git@gitee.com:xxxx/store.git)

3. git add . 

4. git commit -m " "

5. git push origin 分支名（master）

6. push时候可能产生的错误如下：

　　* failed to push some refs to 'git@gitee.com:xxxx/store.git'   错误原因  本地git仓库目录下为空

　　* fatal: refusing to merge unrelated histories  原因：本地仓库和线上仓库不相干   建立强制关联  git pull origin master --allow-unrelated-histories



## 建立公钥（为了解决每次对远程仓库操作都要输入密码的问题）

1. ssh-keygen -t rsa -C  "xxx@xxx.com"  三次回车

2. cat ~/.ssh/id_rsa.pub 获取公钥
