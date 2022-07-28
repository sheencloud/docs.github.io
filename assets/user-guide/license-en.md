# Hyperkuber License许可管理

Hyperkuber的集群管理，用户管理以及资源管理通过License系统控制，Hyperkuber的用户可以通过[sheencloud](https://account.sheencloud.com/sessions/signin)注册用户，后申请或者购买License。

## 注册用户
**方式1:**
打开[sheencloud](https://account.sheencloud.com/sessions/signin)，填写用户名，用户邮箱完成注册。

*用户名：用户的唯一标识
*用户邮箱：用于接受Sheencloud的邮件订阅以及邮件通知

**方式2:**
打开huperkuber web服务的Ingress地址，默认地址是：Hyperkuber.cluster.local,使用默认用户名/密码登陆： admin/Hyperkuber@1314，登陆成功后，显示License注册页面，如下图所示：
![Minion](../../assets/images/license/register.jpg)
填写用户名，用户邮箱完成注册。


## 购买
Hyperkuber的License只能通过SheenCloud的官方网站购买，购买链接[License](https://account.sheencloud.com/service/subscriptions),根据不同的用户需求购买相关产品，付款完成后，用户可以在订阅页面查询到已购买的License。
![Minion](../../assets/images/license/order1.jpg)
Key（LicenseID）： 用于在线激活Hyperkuber相关产品。
![Minion](../../assets/images/license/order2.jpg)
License Data：点击LicenseID进入License的详情页面，可以查看到LicenseData的详细加密数据，LicenseData用于离线激活Hyperkuber相关产品

## 激活
**方式1:在线激活**
打开Hyperkuber web服务的Ingress地址,使用默认账号密码登陆，登陆成功后跳转License激活页面
![Minion](../../assets/images/license/active1.jpg)

注：部署Hyperkuber服务的环境需要能访问SheenCloud官方网站，激活

**方式2:离线激活**
打开Hyperkuber web服务的Ingress地址,使用默认账号密码登陆，登陆成功后跳转License激活页面
![Minion](../../assets/images/license/active2.jpg)
## 申请试用
用户可以免费申请为期14天的免费License，License中包含注册1个集群，1个用户，资源限制1000。
申请方式如注册用户的**方式2**页面相同，打开huperkuber web服务的Ingress地址，用户登陆成功后，显示License注册页面，输入用户名，用户邮箱即可申请免费14天的试用License


