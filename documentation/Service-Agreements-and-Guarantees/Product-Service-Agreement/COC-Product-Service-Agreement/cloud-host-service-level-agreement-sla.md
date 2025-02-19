 本服务等级协议（Service Level Agreement，简称 “SLA”）规定了京东云向客户提供的合作云主机的服务可用性等级指标及赔偿方案。特别提示您，除非另有约定，本协议不适用于公测、邀测的规格类型。

 

**1.** **定义**

**可用区：** 每个地域内电力及网络之间互相独立的物理区域。

**服务周期** ：一个服务周期为一个自然月。

**单实例服务周期总分钟数：** 按照单实例服务周期内的总天数╳24（小时）╳60（分钟）计算。

**实例不可用：** 当一台设置了出入允许规则的实例以TCP或者UDP协议与任一IP地址的双向（出/入）都无法联通，且该状态持续一分钟以上，视为该分钟内实例不可用。

**单实例服务不可用分钟数** ： 在一个服务周期内单实例不可用分钟数之和。

**单地域多可用区服务不可用：** 如用户的实例在同一地域部署于至少2个可用区（以下简称：单地域多可用区），若该地域任一可用区发生该用户的全部实例不可用，且该用户在该地域其他可用区的实例亦同时发生实例不可用，则此同地域其他可用区不可用实例被视为单地域多可用区服务不可用。

**单实例单地域多可用区服务不可用分钟数：** 在一个服务周期内，单实例的 **单地域多可用区服务不可用** 的分钟数之和。

**月度服务费：** 为客户在一个服务周期（即自然月）中就单实例所支付的服务费用总额，如客户一次性支付多个月份的服务费，则将按照所购买的月数分摊计算月度服务费。

**2.** **服务可用性**

**2.1** **服务可用性计算方式**

服务可用性将根据服务周期，按如下两种维度分别统计每台实例的可用性：

 （1）单实例维度：

 服务可用性=（单实例服务周期总分钟数 - 单实例服务不可用分钟数）/单实例服务周期总分钟数×100%

（2）单地域多可用区维度：

服务可用性=（单实例服务周期总分钟数 - 单实例单地域多可用区服务不可用分钟数）/单实例服务周期总分钟数×100%

**2.2** **服务可用性承诺**

（1）对于单实例维度，京东云承诺一个服务周期内云主机的服务可用性不低于99.975%；

（2）对于单地域多可用区维度，京东云承诺一个服务周期内云主机的服务可用性不低于99.995%。

 2.3如未达到上述可用性承诺，客户可以根据本协议第3条约定获得赔偿。**赔偿范围不包括以下原因所导致的服务不可用：**

（1）任何京东云或京东云合作地域所属设备以外的网络、设备故障或配置调整引起的；

（2）客户的应用程序受到黑客攻击而引起的；

（3）客户维护不当或保密不当致使数据、口令、密码等丢失或泄漏所引起的；

（4）客户的疏忽或由客户授权的操作所引起的；

（5）客户未遵循京东云产品使用文档或使用建议引起的，如客户在控制台、API或者CLI等控制方式对实例进行关机、重启、卸载云盘等操作引起的不可用；

（6）使用存储优化型及GPU型等带本地数据盘的实例，其存储在本地盘中的数据有丢失风险，依赖本地盘存储中数据而导致的不可用；

（7）由于运营商故障导致的丢包和延时等不可用情况；

（8）由于客户所安装软件或者其他非京东云直接运营的第三方软件或者配置引起的实例出现错误；

（9）由于客户违反《合作云产品服务条款》导致的服务被暂停或终止；由于欠费、包月到期导致实例被暂停服务或被释放等；

（10）京东云预先通知用户后进行系统维护所引起的，包括割接、维修、升级和模拟故障演练；

（11）不可抗力引起的；

（12）属于相关法律法规、相关协议、相关规则或京东云单独发布的相关规则、说明等中所述的京东云可以免责、免除赔偿责任等的情况。

（13）其他非京东云原因所造成的不可用。

 

**3.** **赔偿方案**

**3.1 赔偿标准** 

（1）对于单实例，如服务可用性低于99.975%，可按照下表中的标准获得赔偿，赔偿方式仅限于用于发放购买云主机产品的代金券，且赔偿的代金券总额不超过未达到服务可用性承诺当月客户就该实例支付的单实例月度服务费金额（不含用免费代金券抵扣的费用）。


| **服务可用性**             | **赔偿代金券金额** |
| -------------------------- | ------------------ |
| 低于99.975%但等于或高于99% | 月度服务费的10%    |
| 低于99%但等于或高于95%     | 月度服务费的25%    |
| 低于95%                    | 月度服务费的100%   |


 （2）对于以单地域多可用区部署的，如服务可用性低于99.995%，可按照下表中的标准获得赔偿，赔偿方式仅限于用于购买云主机产品的代金券，且赔偿总额不超过未达到服务可用性承诺当月，用户就该实例支付的月度服务费（不含用免费代金券抵扣的费用）。

| **服务可用性**             | **赔偿代金券金额** |
| -------------------------- | ------------------ |
| 低于99.995%但等于或高于99% | 月度服务费的10%    |
| 低于99%但等于或高于95%     | 月度服务费的25%    |
| 低于95%                    | 月度服务费的100%   |

 （3）如某实例同时满足3.1（1）和（2）的赔偿标准，则以其中赔偿额较高者为准计算赔偿金额。

 **3.2** **赔偿申请时限**

客户可以在每月第五（5）个工作日后对上个月没有达到可用性的实例提出赔偿申请。 **赔偿申请必须限于在云主机没有达到服务可用性的相关月份结束后两（2）个月内提出。超出申请时限的赔偿申请将不被受理。**

**4.** **其他**

本云主机服务等级协议自2022年9月1日生效，京东云有权对本SLA条款作出修改。如本SLA条款有任何修改，京东云将提前15天以网站公示或发送邮件的方式通知您，生效时间为公示后的下一个服务周期即下一个自然月的第一天。如您不同意京东云对SLA所做的修改，您有权停止使用服务，如您继续使用服务，则视为您接受修改后的SLA。






