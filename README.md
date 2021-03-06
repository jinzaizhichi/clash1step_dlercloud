# Clash for Linux一键安装脚本(支持订阅)
#### 参照油管UP主：米月大佬的灯塔脚本修改的一键安装Clash For Linux。加入了一下功能：
###### 1.支持创建非root用户，以供安装Clash
###### 2.支持机场托管订阅（目前仅测试墙洞）

```
apt install wget -y
```

```
bash <(wget --no-check-certificate -qO- http://uee.me/dbhvv)
```

###### 3.一些操作指令
启动Clash
```
sudo systemctl start clash.service
```
重启Clash
```
sudo systemctl restart clash.service
```
查看Clash运行状态
```
sudo systemctl status clash.service
```
实时滚动状态
```
sudo journalctl -u clash.service -f
```

# 脚本使用注意事项：

## 1.仅支持Debian10.3(其他系统未测试）

## 2.脚本需在root用户下运行，且系统需要配置科学上网环境

## 3.机场托管的配置文件必须配置DNS参数，且必须为Fake-ip模式
### 关于fake-ip的原理，可以看看以下F大跟苏大的文章

#####DNS污染对Clash（for Windows）的影响
###### https://github.com/Fndroid/clash_for_windows_pkg/wiki/DNS%E6%B1%A1%E6%9F%93%E5%AF%B9Clash%EF%BC%88for-Windows%EF%BC%89%E7%9A%84%E5%BD%B1%E5%93%8D

##### 代替 Surge 增强模式——使用 KoolClash 作为代理网关
###### https://blog.skk.moe/post/alternate-surge-koolclash-as-gateway/

##### 浅谈在代理环境中的 DNS 解析行为
###### https://blog.skk.moe/post/what-happend-to-dns-in-proxy/
