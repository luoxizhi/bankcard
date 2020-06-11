# bankcard
离线银行卡识别算法



​        现在主流的银行卡识别都是基于离线模式的，国外有一个card.io开源库，效果很好，但只支持16位凹凸银行卡，不能识别19位的银行卡，而国内大行都是19位卡，Github现状是还没有一个可用的开源离线银行卡识别的项目。

​         本开源库是基于card.io的思路，使用多个CNN模型结合图像处理算法，实现了对16，17，18，19位银行卡的识别，同时支持凹凸银行卡和印刷银行卡，识别率90%，反应时间小于1秒。

1.不需要和服务器交互，避免了法律风险。

2.神经网络和CNN的模型体积小，总共800KB。

3.离线扫描银行卡模块作为 SDK 输出，集成简单。

架构和算法示意图

![image-20200611104032815](https://tva1.sinaimg.cn/large/007S8ZIlly1gfo5h31k1tj30jp09jwgy.jpg)

算法改进效果示例

![image-20200611104147616](https://tva1.sinaimg.cn/large/007S8ZIlly1gfo5ido4laj30ip09hwiy.jpg)

![image-20200611104200862](https://tva1.sinaimg.cn/large/007S8ZIlly1gfo5ilqaazj30i708ydk7.jpg)

