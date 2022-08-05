# 集群角色

集群角色包含表示一组权限的规则。作用范围是跨Namespace。
![Minion](../../../assets/images/system/crole-list.jpg)
## 集群角色操作

![Minion](../../../assets/images/system/crole-operation.jpg)
支持以下界面图形化操作：

* 标签
* 注解
* Yaml/Json编辑

### 创建
创建集群角色，点击“创建集群角色”按钮，进入创建集群角色页面，填写必要参数
![Minion](../../../assets/images/system/crole-create1.jpg)
参数
名称：集群角色名称
规则：
* 资源
* 资源组
* 操作： list get create等操作
### 集群角色详情
点击集群角色名称的链接，即可进入集群角色的详情页面
概览信息
![Minion](../../../assets/images/system/crole-info1.jpg)

Yaml信息
![Minion](../../../assets/images/system/crole-info2.jpg)
集群角色绑定信息
![Minion](../../../assets/images/system/crole-info3.jpg)
事件信息
![Minion](../../../assets/images/system/crole-info4.jpg)


### 删除
选择需要删除的集群角色，点击多选框选择，点击“删除按钮”，在确定输入框输入“yes”，即可完成删除操作。
### 刷新
点击“刷新”，即可完成集群角色列表的刷新。