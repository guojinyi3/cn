## 价格说明

风险识别服务计费形式包括包年不限次、按量资源包和按量后付费。按量资源包支持全品类抵扣。

| 对比项   | 包年不限次资源包                                     | 按量资源包                                               | 按量后付费                             |
| :------- | ---------------------------------------------------- | :------------------------------------------------------- | :------------------------------------- |
| 付费模式 | 预付费，有效期一年                                   | 预付费，有效期一年                                       | 按使用量日结                           |
| 单价     | 单价相对较高，适合年调用量较大或业务高速增长         | 单价较低，购买资源包规格越高，单价越低                   | 单价较高                               |
| 使用场景 | 业务高速发展，预估年调用量大于5000万次，担心超出预算 | 业务相对稳定，可精准预估每年调用量，年调用量小于5000万次 | 资源包消耗完毕或到期，未继续购买的客户 |

#### 定价详情

按量资源包价格

| **资源包规格** | 100万次 | 1000万次 | 3000万次 | 5000万次 |
| :------------: | ------- | -------- | -------- | -------- |
| **价格（元）** | 8000    | 60000    | 150000   | 200000   |

包年资源包价格

| 产品名称包年不限调用次数（有效期1年）单位：万 | QPS上限 10000 | QPS上限 5000 | QPS上限 3000 | QPS上限 1000 | QPS上限 500 | QPS上限 300 | QPS上限 100 |
| --------------------------------------------- | ------------- | ------------ | ------------ | ------------ | ----------- | ----------- | ----------- |
| 号码风险识别                                  | 186.88        | 138.4        | 119.2        | 100          | 95.2        | 92          | 88          |
| IP风险识别                                    | 94.4          | 61.6         | 48.64        | 35.68        | 32          | 30.4        | 28.8        |
| 地址风险识别                                  | 186.88        | 138.4        | 119.2        | 100          | 95.2        | 92          | 88          |
| 注册风险识别-标准版                           | 116.5         | 68           | 49           | 30           | 25.3        | 23.4        | 21.5        |
| 登录风险识别-标准版                           | 116.5         | 68           | 49           | 30           | 25.3        | 23.4        | 21.5        |
| 营销风险识别-标准版                           | 116.5         | 68           | 49           | 30           | 25.3        | 23.4        | 21.5        |
| 注册风险识别-定制版                           | 166.5         | 118          | 99           | 80           | 75.3        | 73.4        | 71.5        |
| 登录风险识别-定制版                           | 166.5         | 118          | 99           | 80           | 75.3        | 73.4        | 71.5        |
| 营销风险识别-定制版                           | 166.5         | 118          | 99           | 80           | 75.3        | 73.4        | 71.5        |

超出资源包的部分采用按使用量后付费，每日结算。**按量计费为每1个抵扣次数0.01元**，比如号码调用一次，就是0.01*8（抵扣系数）=0.08元/次。

抵扣方式（次数）：

| 功能 | 抵扣系数 |
| ---- | -------- |
| 号码 | 8        |
| IP   | 5        |
| 地址 | 8        |
| 注册 | 10       |
| 登录 | 10       |
| 营销 | 10       |


抵扣解释：

1. 抵扣量=调用量 * 抵扣系数。例如，您购买了100万的资源包，号码调用了10万次，则抵扣量=10万 *8=80万次，剩余20万次。
2. 资源包不足以抵扣时，则剩余的调用量将会按照按量付费的价格收费。例如，您已购买3000万次的资源包，资源包剩余600万次，您今天地址调用了100万次，抵扣量=100万次* 8=800万次，抵扣掉资源包后还需抵扣200万次。200万次按照后付费价格（0.01元/次）为您计费，今天还需付费2000000*0.01=20000元。

#### 免费试用

首次开通服务可以领取10000次免费调用额度，一个月内有效。如额度消耗完，没有购买资源包，按使用量后付费，按日扣费。如果欠费，您可以在24小时内结清，在这期间可以继续使用。超过24小时后，停服不能继续使用。
