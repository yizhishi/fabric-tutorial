# fabric tutorial

just wanna build my first fabric network and communicate with my network via fabric-sdk-go.

## build my first network

网络计划使用 raft 共识, 2个org, 每个org下有2个peer.

1. 从 hyperledger-fabric 编译 cryptogen, configtxgen 等二进制文件

2. 自己写 cryptogen 和 configtxgen 所需的配置文件, 共识机制使用 raft

3. 使用 docker-compose 或者 k8s 启动 orderer 和 peer 节点.

## 使用 fabric-sdk-go 与 创建的 fabric network 交互

1. 创建 channel
2. 节点加入 channel
3. update anchor peer
4. install chaincode
5. chaincode instantiate
6. query & invoke chaincode

## 非初始化组织加入

非初始化组织加入 network, 所需的证书通过 fabric-ca-server 的 API 创建, 然后进行加入组织的一系列操作.
