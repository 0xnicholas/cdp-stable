# CDP-stablecoin Experiment

## Summary


## Overview
基于CDP的稳定币实验，具有以下特性：
- 利用L2s构建，统一EVM流动性原生跨链
- (抵押品管理) 抵押品和稳定币可自动转换，用来保护抵押品
- 更多的抵押品种类(Exotic collateral types)，同时了引入了更多风险，则设计一种类保险的抗风险机制
- 动态利率设计
- 通过质押获得收益和积分


## How it works

### $STABL made
> $STABL is created through depositing collateral and opening loans.

STABL是一种基于抵押的稳定币，这就是说STABL的价值由其他资产（如BTC, ETH）的价值支撑，每当有人想要创建STABL时，他们都必须存入一些资产，并将其锁定在智能合约中抵押。存入抵押品以铸造稳定币通常被称为开立抵押债务头寸 (CDP)。
如果抵押品的价值跌破某个阈值，智能合约将自动开始交易部分抵押品，以确保 $STABL 始终由等值的美元支撑。你始终必须存入比铸造金额略多的美元价值抵押品，超额抵押的金额取决于你愿意承担的风险。

> 如果借款人推测未来ETH的价格会上涨，借款人可以用ETH作抵押借入STABL(可杠杆)，将STABL在公开市场上swap，以获得更多的ETH，loop，以获得更多收益。




### Collateral Conversion Model


#### Price segment


### Liquidation


#### Liquidation logic



### Earn


## Architecture


### Core contracts


### Flow of [Collateral] in system


### Flow of $STABLE in system


## Project Structure