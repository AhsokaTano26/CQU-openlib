## 0. 前提  
- 前置知识  
    - [判断您的操作系统和系统架构](../计算机基础/判断您的操作系统和系统架构.md)  
    - [命令行基础](../计算机基础/命令行基础.md)  


## 1. 使用方法
### 1.1 找到系统Hosts文件
- Windows：`C:\Windows\System32\drivers\etc\hosts`  
- MacOS：`/etc/hosts`  
- Linux：`/etc/hosts`  

### 1.2 添加Github到Hosts文件
- 复制以下内容
    ```
    #Github Hosts Start
    140.82.112.26 alive.github.com
    140.82.114.26 live.github.com
    185.199.109.154 github.githubassets.com
    140.82.113.21 central.github.com
    185.199.111.133 desktop.githubusercontent.com
    185.199.110.153 assets-cdn.github.com
    185.199.110.133 camo.githubusercontent.com
    185.199.108.133 github.map.fastly.net
    146.75.121.194 github.global.ssl.fastly.net
    140.82.121.4 gist.github.com
    185.199.108.153 github.io
    140.82.121.4 github.com
    192.0.66.2 github.blog
    140.82.121.6 api.github.com
    185.199.108.133 raw.githubusercontent.com
    185.199.108.133 user-images.githubusercontent.com
    185.199.108.133 favicons.githubusercontent.com
    185.199.111.133 avatars5.githubusercontent.com
    185.199.111.133 avatars4.githubusercontent.com
    185.199.108.133 avatars3.githubusercontent.com
    185.199.111.133 avatars2.githubusercontent.com
    185.199.111.133 avatars1.githubusercontent.com
    185.199.108.133 avatars0.githubusercontent.com
    185.199.109.133 avatars.githubusercontent.com
    140.82.121.10 codeload.github.com
    54.231.225.97 github-cloud.s3.amazonaws.com
    3.5.28.88 github-com.s3.amazonaws.com
    16.15.200.160 github-production-release-asset-2e65be.s3.amazonaws.com
    52.217.94.188 github-production-user-asset-6210df.s3.amazonaws.com
    52.217.91.76 github-production-repository-file-5c1aeb.s3.amazonaws.com
    185.199.110.153 githubstatus.com
    140.82.113.18 github.community
    51.137.3.17 github.dev
    140.82.113.21 collector.github.com
    13.107.42.16 pipelines.actions.githubusercontent.com
    185.199.111.133 media.githubusercontent.com
    185.199.108.133 cloud.githubusercontent.com
    185.199.110.133 objects.githubusercontent.com
    ```
- 添加至 Hosts 文件末尾
    - Windows：使用记事本
    - MacOS：使用命令 `sudo nano /etc/hosts` 编辑
    - Linux：使用命令 `sudo vim /etc/hosts` 编辑

### 1.3 激活生效
大部分情况下是直接生效，如未生效可尝试下面的办法，刷新 DNS：

- Windows：使用命令 `ipconfig /flushdns`
- MacOS：使用命令 `sudo killall -HUP mDNSResponder`
- Linux：使用命令 `sudo nscd restart`
## 2. 提醒
- 如无效果请重启尝试
## 3. 参考链接
[https://github.com/maxiaof/github-hosts](https://github.com/maxiaof/github-hosts)