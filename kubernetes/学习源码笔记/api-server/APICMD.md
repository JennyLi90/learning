# NewAPIServerCommand
kube-apiserver
1. verflag.PrintAndExitIfRequested()
2. utilflag.PrintFlags(cmd.Flags())
3. CreateNodeDialer creates the dialer infrastructure to connect to the nodes.


## CreateServerChain
### CreateKubeAPIServerConfig
参考 https://github.com/yangxikun/yangxikun.github.com/blob/b7a0e5cd224104f6aba1d66a2d83a945496360aa/_posts/2019-12-27-kubernetes-api-server.md

CreateServerChain 创建的3个 Server，都采用了类似 config->complete()->completedConfig->new()->server 的调用完成

## 问题
1. defaultEtcdPathPrefix 干什么用的？

资源信息存储路径前缀缺省为：DefaultEtcdPathPrefix = "registry"
但是这个参数我们可以在运行时指定参数覆盖，具体的参数配置为：etcd-prefix



