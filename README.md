# Clash for Linux一键安装脚本(支持订阅)
#### 参照油管UP主：米月大佬的灯塔脚本修改的一键安装Clash For Linux。加入了一下功能：
###### 1.支持创建非root用户，以供安装Clash
###### 2.支持机场托管订阅（目前仅测试墙洞）

# 脚本使用注意事项：

## 1.仅支持Ddebian10.3(其他系统未测试）

## 2.脚本需在root用户下运行，且系统需要配置科学上网环境

## 3.机场托管的配置文件必须配置DNS参数，且必须为Fake-ip模式


```
apt install wget -y
```

```
bash <(wget --no-check-certificate -qO- http://uee.me/dbhvv)
```

