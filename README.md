minerProxy mp303 原版稳定版 一键安装脚本，

转发模式无开发费，史上最稳定版本，稳定大于一切！转发损耗<0.5%

本仓库仅原版303的一键安装脚本，防火墙+改连接数+自启动守护

矿池代理，支持TCP和SSL协议，支持自定义抽水，高性能高并发，支持web界面管理。 

开发费:


抽水 <= 5% : devfee = 0.3%

抽水 <= 20% : devfee = 1%

抽水 >  20% : devfee = 抽水

安装完成后，请立即修改默认密码，以防别有用心之人，扫描端口偷偷登录！！！ 

安装好之后记得改掉默认的访问端口；文件名是config.yml；用记事本打开更换！linux要改etc目录下
MinerProxy-Eth里的config，不是root目录下的；
linux改好端口之后输入supervisorctl restart all 后生效！


# linux服务器一键安装脚本；自带守护，开放最大连接数
```bash
bash <(curl -s -L http://dd.ma/OTZ2wBa4)
```
# windows版本下载:
[点击下载 ](https://github.com/mp303eth/MinerProxy303/raw/main/minerProxy_3.0.3_windows.exe) 。
# 备用一键脚本
```bash
bash <(curl -s -L https://raw.githubusercontent.com/minerproxyeth/MinerProxy-Eth/main/install.sh)
```
安装后输入supervisorctl restart all 回车生效！

纯转发模式使用后算力截图，算力几乎无损耗。
![img_9.png](img_9.png)



windows服务器

解压缩后复制到服务器，运行“win守护”然后用浏览器访问 “公网ip:你改好的端口”；密码默认:123456789  进入管理界面 

设置你的转发矿池/端口；可选择“不抽水”(自用) 或者“抽水”(分担服务器费用)；

支持LINUX，WINDOWS服务器，支持纯转发和自定抽水比例；包含自启动和进程守护；

还在被所谓的直连\中转IP抽水吗？自建转发；支持SSL加密；高并发，稳定一键搞定！


（如果遇到打不开管理界面，请开放服务器对应的端口）


任何问题可以联系https://t.me/xxx598 


# Liunx-手动安装

git clone https://github.com/minerproxyeth/minerproxy.git 

cd minerproxy

chmod a+x minerProxy_3.0.3_linux 

nohup ./minerProxy_3.0.3_linux & (后台运行，注意：& 也需要复制，运行完再敲几下回车)

tail -f nohup.out (后台运行时查看)




运行成功后访问 IP:提示的port端口 (如：127.0.0.1:提示的端口 注意开放端口；记得修改端口) 进行配置即可。 




### 后台运行时关闭

killall minerProxy_3.0.3_linux

### 后台运行时查看

tail -f nohup.out

