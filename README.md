# 目录
[1、简介](https://github.com/Bao-Ge/MoneyBoom/blob/main/README.md#1%E7%AE%80%E4%BB%8B)

[2、功能介绍](https://github.com/Bao-Ge/MoneyBoom/blob/main/README.md#2%E5%8A%9F%E8%83%BD%E4%BB%8B%E7%BB%8D)

[3、操作指南](https://github.com/Bao-Ge/MoneyBoom/blob/main/README.md#3%E6%93%8D%E4%BD%9C%E6%8C%87%E5%8D%97)

[4、注意事项](https://github.com/Bao-Ge/MoneyBoom/blob/main/README.md#4%E6%B3%A8%E6%84%8F%E4%BA%8B%E9%A1%B9)

[5、费用说明](https://github.com/Bao-Ge/MoneyBoom/blob/main/README.md#5%E8%B4%B9%E7%94%A8%E8%AF%B4%E6%98%8E)

# 1、简介
金钱豹MoneyBoom是一款能对接TradingView的警报信号，然后在指定交易所进行下单的自动交易工具。
支持TradingView的Email警报（免费版TradingView也能进行量化交易），支持币安U本位合约和欧易的U本位合约。
金钱豹工作方式如下图所示。
![0](https://github.com/user-attachments/assets/7780c3fc-04b0-4d60-a22f-bd7da4fab76b)

## 1.1、核心功能
- 对接Tradingview发出的email警报
- 对接币安合约或欧易合约
- 支持设置杠杆和仓位百分比
- 支持多币种交易
- 支持单币种的多策略交易
- 支持2TP交易
- 支持网格交易
- 简单便捷的警报消息配置 

## 1.2、拓展功能
- 显示当前持仓和交易清单
- 对历史交易进行收益分析
- 统计月度收益并曲线显示
- 显示历史余额走势
- 支持手动开仓、平仓
- 账户安全保护，工具复制到另一台电脑，账户失效

# 2、功能介绍

![1](https://github.com/user-attachments/assets/ebae624a-c512-42f9-a62d-89df69d2a6b5)

## 2.1、交易对
选择指定交易对，可进行杠杆、仓位、仓位类型和止损配置；
![6](https://github.com/user-attachments/assets/3f086700-5667-4865-90e9-55e2a9c09cb3)

1. 目前最大支持50x；
2. 仓位为各个交易对占保证金的百分比，如果同时跑BTCUSDT和ETHUSDT，可各设置50%，仓位占比之和为100%；
3. 类型：全仓杠杆和逐仓杠杆；
4. 止损：当亏损达到该值后，将自动进行平仓止损；

## 2.2、账户
币安账号只显示BNB、USDT和BUSD，对于欧易账号只显示USDT；
对于需要BNB显示正确的换算U余额，请在交易对保留BNBUSDT；
建议往币安合约账户里充值BNB，BNB做手续费有优惠；
![13](https://github.com/user-attachments/assets/7edd8993-4868-4c76-b748-4e4b1402a656)

## 2.3、本金与收益
显示当前本金、余额、盈利和收益，其中本金需要手动修改；

盈利 = 余额 - 本金

收益 = 盈利 / 本金

![本金与收益](https://user-images.githubusercontent.com/6885956/167294510-23312bc6-a441-4da4-88bd-a3f4b8a52705.png)

## 2.4、持仓
显示当前持仓信息；

![持仓](https://user-images.githubusercontent.com/6885956/167294511-ec178fa1-0663-4c69-89c8-058bc8d7d066.png)

## 2.5、交易清单
显示当前交易的历史记录，与TradingView完美匹配；
![交易清单](https://user-images.githubusercontent.com/6885956/167294513-8250d58f-b4af-48a1-91bc-22654cdc8411.png)

## 2.6、手动交易
- 选择左上角的交易对，可进行手动交易；
- 在“单交易对多策略”的模式下，若要平掉交易清单的仓位，请修策略代号，与交易清单中的策略代号一致；
- 在“单交易对单策略”的模式下，若要平掉交易清单的仓位，可直接点击“平多”或“平空”；

![手动交易](https://user-images.githubusercontent.com/6885956/167294528-4d2495d3-9993-46de-82e9-3dce735eba94.png)

## 2.7、概览·统计
显示“今日收益”、“累计胜率”和“盈利因子”等相关统计结果，以图表的方式显示每月收益数据；

![概览·统计](https://user-images.githubusercontent.com/6885956/167294522-85957ed3-8bd1-41bf-9ae3-68d5941f0596.png)

## 2.8、信号记录
- 信号：与TradingView一致；
- 源：有webhook、email和Button三种类型，记录当前警报的来源；

![信号记录](https://user-images.githubusercontent.com/6885956/167294525-33b7d1ff-0c9d-4426-9d37-4149096720c2.png)

## 2.9、余额曲线
每次平仓后，会记录当前余额，并绘制曲线；

![余额曲线](https://user-images.githubusercontent.com/6885956/167294526-ff49d6f8-c18b-4aa1-b0ae-4073bc380c0a.png)

## 2.10、状态栏
- 显示当前交易所、Email和Webhook的连接状态；
- 若中途断开连接，则会发送Email通知；

![状态栏](https://user-images.githubusercontent.com/6885956/167293921-94b690b1-a690-4364-a636-a2e4d32fa598.png)

## 2.11、版本信息
当前当前工具版本和license版本；

![版本信息](https://user-images.githubusercontent.com/6885956/167293922-3752dd89-75d0-4a2d-8bc9-61b2f6345c37.png)

# 3、操作指南
用于指导下载、安装和相关配置；
## 3.1、下载、安装

[安装包下载地址](https://github.com/Bao-Ge/MoneyBoom/releases/tag/MoneyBoom)

下载之后，双击“MoneyBoom Setup V2.msi”，默认安装，安装完成后，会生成桌面快捷方式；

如下如所示：

![图标](https://user-images.githubusercontent.com/6885956/167296693-3b38a0f3-cad8-498f-81b1-7ac80c6c2182.png)

双击图标，显示如下：

![首次登录](https://user-images.githubusercontent.com/6885956/167296873-e7942a9d-67da-433c-a397-74db55b83ff9.png)

## 3.2、配置流程
点击上图中左上角的金钱豹图标，进行相关配置；

配置流程如下：

```
    配置邮箱 --> 配置API --> 配置TradingView
```

## 3.3、参数配置
详细配置说明见4.1

![配置界面](https://user-images.githubusercontent.com/6885956/167296759-1e8f1fee-3bb7-4292-b68f-16062bd45907.png)

## 3.4、TradingView警报配置
- ==警报名称：请保持为空==
- webhook URL：请点击参数配置界面中的"webhook地址"，则复制webhook URL；
- 消息：常规警报请点击参数配置界面中的"常规警报指令"；2TP警报则点击“2TP警报指令”；
- 常规警报和2TP警报的区别见4.5；
 
![警报配置](https://user-images.githubusercontent.com/6885956/167297672-0642387a-b5a3-45b1-bccb-064aa7a1b492.png)

## 3.5、激活注册
点击如图所示的图标，进行注册；

![激活](https://user-images.githubusercontent.com/6885956/167298187-205215ab-82b6-460c-b43b-ff7fd1527774.png)

激活步骤如下：

进行注册；

![激活配置](https://user-images.githubusercontent.com/6885956/167298251-450823fe-bde0-45c3-b5a8-641bcd9ab20a.png)
1. 复制机器码，然后再联系我；
2. 复制激活码至红色方框中；
3. 点击“激活”按键，完成激活，同时状态会更新；

![状态更新](https://user-images.githubusercontent.com/6885956/167298600-af030179-7843-4a34-a6f7-9e3cf1d03cb0.png)
license说明请见 “5、费用说明”

## 3.6、添加新账号
点击加号，则可新增账户；

![状态更新](https://user-images.githubusercontent.com/6885956/167298712-d8ee9313-d693-40bf-8f42-c395aedca42a.png)

## 3.7、语言切换
如下图所示，切换图标；

![语言切换](https://user-images.githubusercontent.com/6885956/167298824-b47060c1-27b3-48c8-b373-aa2c6efd804d.png)

# 4、注意事项
在使用MoneyBoom工具之前，请先了解一下相关注意事项；
## 4.1、参数配置说明
### 4.1.1、邮箱配置
推荐使用QQ邮箱，QQ邮箱能够和微信绑定，能即使收到消息；

登录QQ邮箱，点击设置，切换到账户；

![邮箱配置](https://user-images.githubusercontent.com/6885956/167299071-3a40b94e-d992-4600-8b8f-009c0ea94e30.png)
开通IMAP/SMTP,生成授权码，授权码即为邮箱的登录密码；

![授权码](https://user-images.githubusercontent.com/6885956/167299112-b47e5401-66f0-43e0-9268-4f8cc19f7691.png)

### 4.1.2、币安API
登录币安网页版，获取API Key 和 API Secret;
### 4.1.3、欧易API
登录欧易网页和APP，获取V5 API Key 和 API Secret;

### 4.1.4、策略模式
- 单交易对单策略模式：如BTCUSDT只能运行一个策略，若运行多个，则各个策略的仓位会相互影响，优点是工具的webhook信号、工具的手动交易和在APP上的交易，能够相互开仓、平仓；
- 单交易对多策略模式：如BTCUSDT能运行多个策略，则各个策略的仓位相互独立；

![策略模式](https://user-images.githubusercontent.com/6885956/167299424-0bc8d5f0-2ded-4c15-8e46-fe9352f2a1c3.png)

### 4.1.5、报警码
不同账户之间可用报警码区分，如币安用M1,欧易用M2，当我们配置警报时，可用报警码区分，若币安用M1,欧易也用M1，则配置一个报警，币安和欧易同时进行交易；

### 4.1.6、网络配置
- ****海外服务器****
HTTP地址会自动获取，勾选使用webhook；

![海外服务器](https://user-images.githubusercontent.com/6885956/167299914-a4843eaf-97cd-4983-9090-4f01a44064e2.png)
- **科学上网版**
HTTP地址，请输入花生壳的内网穿透地址；

代理地址，请输入科学上网工具地址，主要是需要找到代理端口；

![科学上网版](https://user-images.githubusercontent.com/6885956/167299959-7faeb6b4-db64-4a55-91a6-431c27a537c9.png)
- **无TradingView会员**
支持邮件解析警报信号，适合白嫖党；

HTTP地址，请输入花生壳的内网穿透地址；

代理地址，请输入科学上网工具地址，主要是需要找到代理端口；

![无TradingView会员](https://user-images.githubusercontent.com/6885956/167299978-4c370665-4fb5-4fa9-b70d-760d215f8a75.png)

## 4.2、警报配置说明
警报消息如下所示，适用于TradingView的所有策略；

警报中的占位符说明，请看

[https://cn.tradingview.com/chart/?solution=43000531021](com/)[link](com/)

其中M1为报警码，XXXXX为策略代号，100为改策略的仓位占比；
- **常规警报**
M1:XXXXX,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}},100,{{strategy.order.id}}

- **2TP警报**
M1:XXXXX,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}},50,{{strategy.order.id}},4,{{strategy.order.contracts}},{{strategy.prev_market_position_size}}

## 4.3、Webhook与Email警报说明
 将**常规警报**或 **2TP警报**复制到警报的消息中；
 
 ![警报配置](https://user-images.githubusercontent.com/6885956/167297672-0642387a-b5a3-45b1-bccb-064aa7a1b492.png)
## 4.4、仓位百分比
MoneyBoom里面有2个仓位百分比，一个是交易对的仓位占比，一个是策略的仓位占比；

交易对的仓位占比如下图所示；

![交易对](https://user-images.githubusercontent.com/6885956/167293908-b3642589-d462-4489-862b-e172d2d087e4.png)

策略的仓位占比见高亮的100；

M1:XXXXX,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}},100,{{strategy.order.id}}

见信号记录的仓位；

![信号记录](https://user-images.githubusercontent.com/6885956/167294525-33b7d1ff-0c9d-4426-9d37-4149096720c2.png)

举例说明：

若仓位百分比设置为70%，策略仓位百分比为50%，则实际执行交易的时候，则占用保证金为70%*50%=35%；

需要注意的是在执行交易时，会留些余量，即实际执行的保证金占比为35%*98%=34.3%；

## 4.5、什么是2TP交易
策略介绍如下

[https://cn.tradingview.com/script/VCBUQqGh-JaZYoN-bot-4X-Strategy/](https://cn.tradingview.com/script/VCBUQqGh-JaZYoN-bot-4X-Strategy/)

JaZYoN_bot_4X - Strategy是一个非常优秀的策略，该策略能根据相关指标自动调整杠杆，并且有2个止盈点；如下图所示，信号有2个，合约数为杠杆；

![2TP-1](https://user-images.githubusercontent.com/6885956/167301349-4be42138-ae36-4b51-845b-6f33b1b5a214.png)

![2TP-2](https://user-images.githubusercontent.com/6885956/167301497-00feeaeb-2937-467f-9f52-1d5aa372e2e2.png)

MoneyBoom已完美支持该策略，并且只需要一个警报，即可完成交易，相对于AutoView需要12个警报才能实现该策略，MoneyBoom实在是太方便了，警报信号如下所示；

M1:XXXXX,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}},50,{{strategy.order.id}},4,{{strategy.order.contracts}},{{strategy.prev_market_position_size}}

## 4.6、清空记录
首次使用时，若有开仓，请先平仓，然后点击按键“清空记录”；

## 4.7、使用到期问题
当PRO、PRO+、PREM使用过期后，将会变为FREE版，此时会限制保证金；

# 5、费用说明
| 版本 | FREE | PRO | PRO+ | PREM |
| --- | --- | --- | --- | --- |
|交易保证金限额  | 100 USDT | 100000 USDT | 100000 USDT | 无限制 |
| 允许账户登录数 | 1个 |1个  |5个  |5个  |
| 每月 | 免费 |25 USDT  | 50 USDT | 免费 |
| 每年 | 免费 |278 USDT  | 498 USDT | 免费 |

PREM版本使用条件，使用我的邀请码注册新用户，即可免费使用MoneyBoom金钱豹；

使用邀请码注册还有一个好处就是：交易所会返回20%的交易手续费，咱俩各返10%；

币安邀请链接：[https://accounts.binance.com/zh-CN/register?ref=156555824](https://note.youdao.com/)

币安邀请码：156555824

欧易邀请链接：[https://www.ouyicn.men/join/9464743](https://note.youdao.com/)

欧易邀请码：9464743

## 5.1、收款地址
USDT 收款地址：  0x838944716b526f2c573207def45cb73e1cc80e38

主网：BNB Smart Chain(BEP20)或Ethereum(ERC20)

二维码收款地址

![USDT](https://user-images.githubusercontent.com/6885956/167302999-70256a6c-68b8-472c-8c0b-8ea67c2183bb.png)

## 5.2、交流群
金钱豹电报交流群，大家如果有问题可以随时反馈！

![Telegram](https://user-images.githubusercontent.com/6885956/167303682-47d5c7f5-83c5-4338-9cff-803404efb1a3.png)
