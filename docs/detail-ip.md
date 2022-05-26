
#### IP画像

对于蜜罐捕获到的每个IP，我们会生成一个IP画像，用于您做更深层的IP画像分析。

对于HFish捕获到的所有情报，我们会全部开放给HFish社区用户，完成社区情报的自生产和使用。



在攻击来源页面中，点击详情按钮，即可进到每一个IP的IP情报中。

![image-20220526111406301](http://img.threatbook.cn/hfish/image-20220526111406301.png)



在上部，除了通过整合情报与网络数据，提供HFish综合情报标签以外，我们提供云端规则的攻击行为检出次数和本地威胁检测模块的攻击行为检出次数，进行直观的IP威胁等级参考。

![image-20220526111541932](http://img.threatbook.cn/hfish/image-20220526111541932.png)



此外，针对所有IP，我们会汇聚整个HFish社区捕获到的**IP溯源情报和IP设备信息**。

在这里，即使这个IP攻击单个HFish用户时候没有被抓住有用信息或者溯源，但**只要有一个社区用户捕获到，那么情报信息将在社区内流通与共享。**



最后，根据被攻击的情况，我们又区分了云端IP画像和本地IP画像

在云端画像中，我们可以

**通过他的攻击行为判定他的威胁程度**

假若基本都是中高行为的话，那么我们就可以提高警惕

**通过他的蜜罐攻击情况判定他的针对性**

如果有IP专门攻击vpn的话，那么不消说，他大概率有相关漏洞

**通过他的攻击热力图判定他是人工还是脚本，是不是特殊时间点才开始发起攻击**

如果有从攻防演练开始有攻击记录的IP的话...

![image-20220526112040812](http://img.threatbook.cn/hfish/image-20220526112040812.png)



在云端画像中，我们可以

**查看他具体都在攻击什么节点**

是否对某些节点有针对性

**查询这个IP的所有本地攻击记录链条**

攻击时间链条最短是30天，不限制全长。会展示数据库内所有数据，呈现直观展示。

![image-20220526112130356](http://img.threatbook.cn/hfish/image-20220526112130356.png)





最后，如果有用户因为外网ip测试，导致ip被给了恶意标签的话，可以邮件Honeypot@threatbook.cn说明情况。
