# Pod

Pod 是可在 Kubernetes 中创建和管理的最小可部署计算单元。
![Minion](../../../assets/images/workload/pod-list.jpg)
## Pod操作

![Minion](../../../assets/images/workload/pod-operation.jpg)
支持以下界面图形化操作：
* 调试Pod
* 服务公开
* 镜像升级
* 容忍
* 标签
* 注解
* Yaml/Json编辑

### 状态选择
Pod支持以下状态选择

![Minion](../../../assets/images/workload/pod-status.jpg)

### 命令行
Pod点击“命令行”按钮，弹出“命令行”窗口，可以在“命令行”窗口执行shell命令
![Minion](../../../assets/images/workload/pod-terminal.jpg)

### 日志
Pod点击“日志”按钮，可以查看Pod中Container日志
![Minion](../../../assets/images/workload/pod-log.jpg)

### 创建
创建Pod，点击“创建Pod”按钮，进入创建Pod页面，填写必要参数
![Minion](../../../assets/images/workload/pod-create1.jpg)
参数
名称：Pod名称

![Minion](../../../assets/images/workload/pod-create2.jpg)
参数
镜像名称：Pod镜像名称
镜像地址：Pod镜像仓库地址
暴露端口：服务暴露端口
![Minion](../../../assets/images/workload/pod-create3.jpg)
非必填参数：
Pod安全
Pod网络
其他
点击“创建”即可。

### Yaml创建
Pod可通过Yaml文件直接创建
![Minion](../../../assets/images/workload/pod-create-yaml.jpg)
### Pod详情
点击Pod名称的链接，即可进入Pod的详情页面
概览信息
![Minion](../../../assets/images/workload/pod-info1.jpg)

Yaml信息
![Minion](../../../assets/images/workload/pod-info2.jpg)
容器信息
![Minion](../../../assets/images/workload/pod-info3.jpg)
存储卷信息
![Minion](../../../assets/images/workload/pod-info4.jpg)
环境信息
![Minion](../../../assets/images/workload/pod-info5.jpg)
日志
![Minion](../../../assets/images/workload/pod-info6.jpg)
终端
![Minion](../../../assets/images/workload/pod-info7.jpg)
事件信息
![Minion](../../../assets/images/workload/pod-info8.jpg)
Pod监控信息
![Minion](../../../assets/images/workload/pod-info9.jpg)
### 删除
选择需要删除的Pod，点击多选框选择，点击“删除按钮”，在确定输入框输入“yes”，即可完成删除操作。
### 刷新
点击“刷新”，即可完成Pod列表的刷新。

