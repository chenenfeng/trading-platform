## Overview: https://blog.quantinsti.com/algorithmic-trading-system/
## Helpful: https://blog.quantinsti.com/trading-systems-architecture/
## Order Management Architecture: https://blog.quantinsti.com/automated-trading-order-management-system/
## System Architecture Components
- Market Adapter  -> Data Feed
- Complex Event Processing Engine  -> Strategy
- Order Routing System -> Execution

## What they need to do
market data vendor(like Exchange) provide API that you can change the format

Event Processing Engine: do various statistical calculations, comparison with historical data and decision making


## Several Architectures
1. receive and send
receive market data and send order requests then receive the response from exchange
database -> historical data
database -> trading decision  : study from past trade
three components: 
- exchange
- server: market data receiver, store historical data, store orders from user
- application: receive inputs like placing order, interface for viewing data and orders, order manager interact with exchange

2. New architecture
automated trade need more fast processing speed, like milliseconds and microseconds, also risk management
- change:
1. fast: Complex Event Processing(CEP) move from application to server
2. risk check are performed in the Risk Management System(RMS) within the Order Management(OM)

## Standard Protocal: Financial Information Exchange(FIX）Protocal
so new data vendor show up

## What I should design and code
- Market Data Receiver and Database to store
- CEP engine（Quantopian)  Important and Difficult, also need UI
- Order Management( Including RMS）
