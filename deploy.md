# Avalanche本地部署L1

参考资料：https://build.avax.network/docs/tooling/create-avalanche-l1

## 详细过程

1、安装最新版本的avalanche-cli
```
curl -sSfL https://raw.githubusercontent.com/ava-labs/avalanche-cli/main/scripts/install.sh | sh -s
```
![deploy](./public/1.png)

2、添加系统路径
```
export PATH=~/bin:$PATH
```
3、验证是否安装成功
```
avalanche -h
```
![verify](./public/2.png)

4、创建Avalanche L1配置，可以选择EVM或者其他可定制的VM
```
avalanche blockchain create [链名称]
```
![creat](./public/3.png)
5、节点验证模式，Explain the difference可以诠释两者的区别
![mode](./public/4.png)
6、地址使用默认的，并且选择测试环境
![test](./public/5.png)
7、输入专属的Chain ID，可以通过chainlist官网查看Chain ID是否重复
![chainid](./public/6.png)
8、输入Token的代币名称
![token](./public/7.png)
9、部署L1，选择本地网络
```
avalanche blockchain deploy alfred
```
![localnetwork](./public/8.png)
会自动安装avalache的go语言客户端
![go](./public/9.png)
10、部署成功
![success](./public/10.png)
11、Metamask钱包，使用RPC添加本地部署的L1网络
![rpc](./public/11.png)
12、使用私钥添加默认创建的钱包
![secrect](./public/12.png)
13、添加后就可以看到拥有100W Token的钱包了，可以进行空投或其他后续活动
![wallet](./public/13.png)