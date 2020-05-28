
# build my first network

## 0. 写在前面

略去 go, docker 等其他依赖的安装, 以及使用[fabric源码](https://github.com/hyperledger/fabric)编译二进制文件的过程, 建议先

## 1. 系统初始化

使用 cryptogen 根据 crypto-config.yaml 生成每个组织的 Peer, Orderer 节点账号和组的初始用户账号

``` sh
# 获取默认的配置
cryptogen showtemplate >crypto-config-default.yaml

cp crypto-config-default.yaml crypto-config.yaml

# 修改crypto-config.yaml
vim crypto-config.yaml
```

2. Orderer
