
# Contents

# 1、Introduction
Moneyboom is a tool that can connect with the alarm signal of tradingview and then trade on a designated exchange; Tradingview's webhook and email alerts have been supported. The supported exchanges include binance contract and okex contract.

![MoneyBoom-4](https://user-images.githubusercontent.com/6885956/168480610-5cf7c1c1-e334-4644-b821-2ebd12b2ba65.png)

## 1.1 core functions

- Connect webhook alarm or email alarm sent by tradingview

- Can be long or short in binance contract or okex contract

- Support setting lever and position percentage

- Support multi symbol

- Support multi strategy in single symbol

- Support 2tp strategy

- Simple and convenient alarm message configuration

- One alarm can execute multiple accounts



## 1.2. Expand functions

- Displays the list of current positions and transactions

- Conduct revenue analysis on historical transactions

- Statistics of monthly income and curve display

- Show historical balance trend

- Support manual opening and closing

- For the security protection of the account, the original configuration will become invalid after the tool is copied to other computers
- 
# 2、Function

![MoneyBoom-1](https://user-images.githubusercontent.com/6885956/168481012-f36af8c8-f4e4-428c-adc7-a066ad67b78d.png)

##2.1. Symbol

Select a symbol to configure leverage, position, position type and stop loss;

![Symbol](https://user-images.githubusercontent.com/6885956/168481016-da7c0704-de07-48bf-86b9-ae737ec885d7.png)

1. At present, the maximum support is 10x. We still have to pay attention to risks;

2. The position is the percentage of each symbol in the margin. If btcusdt and ethusdt are run at the same time, 50% can be set respectively, and the sum of positions is 100%;

3. Margin: crossed or isolated;

4. Stop loss: when the loss reaches this value, the position will be closed to stop loss;

##2.2 Account

Only BNB,usdt and busd are displayed for binance account, and only usdt is displayed for okex account;

If BNB is required to display the correct converted u balance, please add bnbusdt to the Symbols;

![Account](https://user-images.githubusercontent.com/6885956/168481943-8d101b07-1bdd-4d33-b9af-ed0c0e218931.png)

## 2.3 Capital and Profit

Display the current Capital, balance, profit and rate, in which the Capital needs to be modified manually;

Rate = Balance - Capital

Income = profit / Capital

![Capital Profit](https://user-images.githubusercontent.com/6885956/168482059-bbdb85d2-b719-46d1-bd8b-566665a09be2.png)

## 2.4、Positions
Display current position information;

![position](https://user-images.githubusercontent.com/6885956/168482197-5cc797be-7e81-4b63-b83d-0eb61f9fa288.png)

## 2.5、TradeHistory
Display the history of the current Trade, which perfectly matches the tradingview;
![TradeHistory](https://user-images.githubusercontent.com/6885956/168483811-f48fda97-fa9f-4502-a5fe-bfe2c447db42.png)

## 2.7、Overview · Statistics
Display relevant statistical results such as "today profit", "7today profit" and "profit factor", and display monthly revenue data in the form of chart;

![overview·Statistics](https://user-images.githubusercontent.com/6885956/168481042-468600c9-282f-4b33-aa06-de8c710b2b3a.png)

## 2.8、Signal
- Signal: consistent with tradingview;

- Source: there are three types: webhook, email and button, which record the source of the current alarm;

![Signal](https://user-images.githubusercontent.com/6885956/168481044-ba8947eb-e36a-4f68-8980-385734636748.png)

## 2.9、Curve
After each closing, the current balance will be recorded and the curve will be drawn;

![Curve](https://user-images.githubusercontent.com/6885956/168481046-de52f986-82b0-4105-871c-0f5754dd145b.png)

## 2.10、Status Bar
- Display the connection status of the current exchange, email and webhook;

- If the connection is disconnected halfway, an email notification will be sent;

![Status Bar](https://user-images.githubusercontent.com/6885956/168482775-6efdc1be-a182-4d0e-9cdf-57888b3c17c3.png)

## 2.11、Version
Current tool version and license version；

![Version](https://user-images.githubusercontent.com/6885956/168482741-1710a3e9-1ea0-429c-acf2-896e7f042a9e.png)

# 3、Manual
Used to guide download, installation and related configuration;
## 3.1、Download And Install

[https://github.com/Bao-Ge/MoneyBoom/releases/tag/MoneyBoom](https://github.com/Bao-Ge/MoneyBoom/releases/tag/MoneyBoom)

After downloading, double-click "moneyboom setup v2. MSI" to install by default. After installation, a desktop shortcut will be generated;

![icon](https://user-images.githubusercontent.com/6885956/167296693-3b38a0f3-cad8-498f-81b1-7ac80c6c2182.png)



## 4、Alarm configuration description

The alert message is as follows, applicable to all policies of tradingview;

See the placeholder description in the alert;

[https://cn.tradingview.com/chart/?solution=43000531021](https://cn.tradingview.com/chart/?solution=43000531021)


M1 is the alarm code, xxxxx is the strategy code, and 100 is the position proportion of the changed strategy;

- **General Alarm**
M1:XXXXX,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}},100,{{strategy.order.id}}

- **2TP Alarm**
M1:XXXXX,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}},50,{{strategy.order.id}},4,{{strategy.order.contracts}},{{strategy.prev_market_position_size}}

## 4.3、Alert Description
 Copy "General Alarm"  or "2TP Alarm" to the alarm message;
 
 ![Alert Description](https://user-images.githubusercontent.com/6885956/168483431-ae73baae-adec-498d-8c8a-01c98b89d9fc.png)
## 4.4、Position percentage
There are two position percentages in moneyboom, one is the position proportion of symbols, and the other is the position proportion of strategies;

The position proportion of transaction pairs is shown in the figure below;

![Symbol](https://user-images.githubusercontent.com/6885956/168481016-da7c0704-de07-48bf-86b9-ae737ec885d7.png)

The position proportion of the strategy is shown in the 100;

M1:XXXXX,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}},100,{{strategy.order.id}}

See the position recorded by the signal;

![signal](https://user-images.githubusercontent.com/6885956/168483706-1fc87221-8b8c-4b83-ad57-08d032500003.png)


Examples：

For example, if the percentage of positions is set to 70% and the percentage of strategy is 50%, the occupied margin will be 70% * 50% = 35% when the transaction is actually executed;

It should be noted that when executing transactions, some margin will be left, that is, the proportion of actually executed margin is 35%*98%=34.3%；

## 4.5、What is a 2TP
The strategy is described below

[https://cn.tradingview.com/script/VCBUQqGh-JaZYoN-bot-4X-Strategy/](https://cn.tradingview.com/script/VCBUQqGh-JaZYoN-bot-4X-Strategy/)

JaZYoN_ bot_ 4X - strategy is a very excellent strategy, which can automatically adjust the lever according to relevant indicators, and has two profit stop points; As shown in the figure below, there are 2 signals, and the number of contracts is leverage;

![2TP-1](https://user-images.githubusercontent.com/6885956/167301349-4be42138-ae36-4b51-845b-6f33b1b5a214.png)

![2TP-2](https://user-images.githubusercontent.com/6885956/167301497-00feeaeb-2937-467f-9f52-1d5aa372e2e2.png)

Moneyboom has perfectly supported this strategy, and only one alarm is needed to complete the transaction. Compared with autoview, it needs 12 alarms to realize this strategy, moneyboom is very convenient. The alarm signals are as follows;

M1:XXXXX,,{{ticker}},{{close}},{{strategy.order.action}},{{strategy.market_position}},{{strategy.prev_market_position}},50,{{strategy.order.id}},4,{{strategy.order.contracts}},{{strategy.prev_market_position_size}}
