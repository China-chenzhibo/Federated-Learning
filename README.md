# Federated-Learning
* 标签：`联邦学习` `新手教程` `虚拟机`
* Label：`Federated Learning` `Tutorial` `Virtual Machine`


## 理论
* 理解联邦学习先看下webank发的白皮书 <br>
* 然后在微信读书里面看《联邦学习》从而对联邦学习有个大致的了解 <br>
* 在github上看大神的FATE框架的readme 看下[如何开始安装使用FATE](https://www.infoq.cn/article/AoQLsGxc4bzvOKheJsAX) ，对于我这种新手最好是使用KubeFATE的Docker-Compose作为部署<br>
* 理解什么是[docker容器](https://www.zhihu.com/question/28300645) <br>

## 实操
* 感兴趣可以看下我在知乎写过的 [联邦学习KubeFATE +Docker Compose的部署及测试（新手篇）](https://zhuanlan.zhihu.com/p/337458436)，这里就不重复展开。 <br>

摘要：<br>

    写在前面：这是我们研究生一门金融基建的课外项目，我们team当时选的是将联邦学习Federated Learning应用到虚拟银行上，用的是微众的FATE开源框架，这篇文章用来讲述怎么部署环境。FATE的部署方式有很多，可以参考官网，但是官网对新手很不友好，解释不够详细，所以我重述一遍。我的需求是两台机器模拟两方，因此用的是KubeFATE +Docker Compose方式。
    * 首先，说明下有些步骤不是必须的，比如如果是在阿里云上开发，那就不用修改阿里云源，或者你能接受那个下载速度也可以；免密登录也不是必须的。大家要斟酌下哈，因为大家的配置不一定是一样的，这里我发一下我的本地配置：hp 64 位 Win10，八核 i7-6700HQ ，内存 8.00 GB。
    * 我是建议大家在阿里云或者AWS上开两台虚拟机，我一开始用的VMware在本地开的两台虚拟机，各自分配了2核2G内存100G硬盘，但是不知道为什么，跟着步骤走，出了很多不可描述的问题，后面在云上开了虚拟机，就顺畅起来了，查资料，有大神说是内存问题，需要给足够的内存给FATE。
    ...
