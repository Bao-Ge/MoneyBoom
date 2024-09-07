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
![交易对](https://github.com/user-attachments/assets/6430d672-3d56-47ed-8c33-c38ca488d256)

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

![本金与收益](https://github.com/user-attachments/assets/7b47b912-e42a-46c2-bb21-316e9c9c9eb7)

## 2.4、持仓
显示当前持仓信息；

![持仓](https://github.com/user-attachments/assets/2cb6bd95-2cc3-4bfc-89ab-6827cc824336)

## 2.5、交易清单
显示当前交易的历史记录，与TradingView完美匹配；

![交易清单](https://github.com/user-attachments/assets/2236ebc0-b64f-4461-99cd-d9834dc72457)

## 2.6、手动交易
- 选择左上角的交易对，可进行手动交易；
- 在“单交易对多策略”的模式下，若要平掉交易清单的仓位，请修策略代号，与交易清单中的策略代号一致；
- 在“单交易对单策略”的模式下，若要平掉交易清单的仓位，可直接点击“平多”或“平空”；

![手动](https://github.com/user-attachments/assets/5f4997c8-805b-4223-a583-208d145400e9)

## 2.7、概览·统计
显示“今日收益”、“累计胜率”和“盈利因子”等相关统计结果，以图表的方式显示每月收益数据；

![统计](https://github.com/user-attachments/assets/561dad04-a9e6-4197-b139-de817fad61a2)

## 2.8、信号记录
- 信号：与TradingView一致；
- 源：Email、Grid-x和Button三种类型，记录当前警报的来源；

![信号记录](https://github.com/user-attachments/assets/ad60aa42-dc59-45b0-9c23-d99d36bf6bb4)

## 2.9、余额曲线
每次平仓后，会记录当前余额，并绘制曲线；

![余额](https://github.com/user-attachments/assets/2aa3b3f2-4a69-4cff-bf0b-5d28739e6b34)

## 2.10、状态栏
- 显示当前交易所和Email的连接状态；

![状态](https://github.com/user-attachments/assets/66bec7ae-5343-43f1-953e-8f069dbf398c)

## 2.11、版本信息
当前当前工具版本；

![版本](https://github.com/user-attachments/assets/bfb6b5b6-dc6c-4765-9423-f9a1c4e95a45)

# 3、操作指南
用于指导下载、安装和相关配置；
## 3.1、下载、安装

[安装包下载地址](https://github.com/Bao-Ge/MoneyBoom/releases/tag/MoneyBoom)


## 3.2、配置流程
点击上图中左上角的金钱豹图标，进行相关配置；

配置流程如下：

```
    配置邮箱 --> 配置API --> 配置TradingView
```

## 3.3、参数配置
详细配置说明见4.1

![参数配置](https://github.com/user-attachments/assets/25d3492c-8406-4926-aea6-a56b0bcdda9d)

## 3.4、TradingView警报配置
- ==警报名称：请保持为空==
- 消息：常规警报请点击参数配置界面中的"常规警报指令"或"常规警报指令+网格"；2TP警报则点击“2TP警报指令”或“2TP警报指令+网格”；
 
![TV设置](https://github.com/user-attachments/assets/eb60ee27-05cb-42fe-b580-93eafe00e7c0)
![TV通知](https://github.com/user-attachments/assets/fd96e6c1-8c00-4693-a1ec-802a127261c6)

## 3.5、激活注册
点击如图所示的图标，进行注册；

![激活](https://github.com/user-attachments/assets/c3e949e4-0fdb-4dee-9e6e-0903dc283d52)


# 4、注意事项
在使用MoneyBoom工具之前，请先了解一下相关注意事项；
## 4.1、参数配置说明
### 4.1.1、邮箱配置

![邮箱密码](https://github.com/user-attachments/assets/c3d925ad-498a-4b68-ae4e-4330f4757f45)

使用Gmail邮箱时，需要注意，不能使用邮箱密码，应使用应用专用密码，获取方法如下：
- 点击邮箱所有设置
  
![邮箱所有设置](https://github.com/user-attachments/assets/2b9e3e28-0f4d-4306-bf24-415e124094e9)

- 启动IMAP
  
![启用IMAP](https://github.com/user-attachments/assets/c01100f7-b4f9-4271-a295-8a6b08f0809c)

- 管理google账户

![管理google账户](https://github.com/user-attachments/assets/ce773098-e90f-4ed5-937a-e9c756c28ccc)

- 两步验证

![两步验证](https://github.com/user-attachments/assets/09ab57b0-4fc1-4d79-a48f-654cdfa8306d)

- 获取应用专用密码

![应用专用密码](https://github.com/user-attachments/assets/8da7d800-4aa0-4ab6-8dd4-9c7f2cc69d7e)

### 4.1.2、币安API
登录币安网页版，获取API Key 和 API Secret;
### 4.1.3、欧易API
登录欧易网页和APP，获取V5 API Key 和 API Secret;

### 4.1.4、策略模式
- 单交易对单策略模式：如BTCUSDT只能运行一个策略，若运行多个，则各个策略的仓位会相互影响，优点是工具的Email信号、工具的手动交易和在APP上的交易，能够相互开仓、平仓；
- 单交易对多策略模式：如BTCUSDT能运行多个策略，则各个策略的仓位相互独立；

### 4.1.5、报警码
TradingView与金钱豹的报警码一致，金钱豹才会认为是有效信号；

## 4.2、警报配置说明
警报消息如下所示，适用于TradingView的所有策略；

警报中的占位符说明，请看

[https://cn.tradingview.com/chart/?solution=43000531021](com/)[link](com/)

其中M1为报警码，XXXXX为策略代号，100为改策略的仓位占比；
- **常规警报**
M1:TEST,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}},100,{{strategy.order.id}}

- **2TP警报**
M1:TEST,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}},50,{{strategy.order.id}},3,{{strategy.order.contracts}},{{strategy.prev_market_position_size}}

- **常规警报+网格**
M1:TEST,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}},50,{{strategy.order.id}},Grid:TEST2,1.005,0.975,5,15

- **2TP警报+网格**
M1:TEST,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}},25,{{strategy.order.id}},3,{{strategy.order.contracts}},{{strategy.prev_market_position_size}},Grid:TEST2,1.005,0.975,5,15

## 4.3、Email警报说明
 将**常规警报** 、 **2TP警报** 、 **常规警报+网格** 或 **2TP警报+网格** 复制到警报的消息中；
 
## 4.4、仓位百分比
金钱豹里面有2个仓位百分比，一个是交易对的仓位占比，一个是策略的仓位占比；

交易对的仓位占比如下图所示；

![交易对](https://user-images.githubusercontent.com/6885956/167293908-b3642589-d462-4489-862b-e172d2d087e4.png)

策略的仓位占比见高亮的50；

M1:XXXXX,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}}, **50** ,{{strategy.order.id}}

举例说明：

若仓位百分比设置为70%，策略仓位百分比为50%，则实际执行交易的时候，则占用保证金为70%*50%=35%；


## 4.5、什么是2TP交易
且有2个止盈点，一个止损点，合约数为为仓位百分数，即根据成交量也会调整仓位；

## 4.6、清空记录
首次使用时，若有开仓，请先平仓，然后点击按键“清空记录”；

## 4.7、使用到期问题
当PRO版本使用过期后，将会变为FREE版，此时会限制保证金；

# 5、费用说明
| 版本 | FREE | PRO |
| --- | --- | --- |
|交易保证金限额  | 100 USDT | 无限制  |
| 每月 |    免费   |  25 USDT  |
