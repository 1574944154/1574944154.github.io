---
title: centos7 yum安装mysql
---


## rpm -ivh https://repo.mysql.com//mysql80-community-release-el7-6.noarch.rpm

## yum install mysql-community-server -y


## 遇到的问题
Downloading packages:
warning: /var/cache/yum/x86_64/7/mysql80-community/packages/mysql-community-icu-data-files-8.0.29-1.el7.x86_64.rpm: Header V4 RSA/SHA256 Signature, key ID 3a79bd29: NOKEY
Retrieving key from file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql-2022


GPG key retrieval failed: [Errno 14] curl#37 - "Couldn't open file /etc/pki/rpm-gpg/RPM-GPG-KEY-mysql-2022"
### 解决方式
修改/etc/yum.repos.d/mysql-community.repo文件
gpgcheck=0