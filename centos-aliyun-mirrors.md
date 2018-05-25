
# how to use aliyun mirrors in china

## how

```bash

# change dir
cd /etc/yum.repos.d/

# backup Centos-Base.repo
mv CentOS-Base.repo CentOS-Base.repo.backup

#get repo files from mirrors.aliyun.com
wget -O CentOS-Base.repo http://mirrors.aliyun.com/repo/Centos-7.repo

# clean yum
yum clean all

# make cache
yum makecache
```
