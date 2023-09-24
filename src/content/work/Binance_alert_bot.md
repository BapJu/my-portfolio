---
title: Binance alert bot
publishDate: 2022-10-02 00:00:00
img: /assets/alert_binance.jpg
img_alt: Soft pink and baby blue water ripples together in a subtle texture.
description: |
  To design and implement an alert system that provides real-time notifications on the positions of top traders on Binance's Futures trading platform.
tags:
  - Python
  - API
---
## Overview

With the burgeoning growth of cryptocurrency trading, keeping an eye on the strategies of top-performing traders can be invaluable. This project leverages Binance's API, identified after a thorough analysis of the platform using Burp Suite, to monitor the positions of leading traders and dispatch timely alerts to clients, aiding them in making informed trading decisions.

## Key Features

1. **Data Acquisition**: Utilizes Binance's API which provides real-time trading positions of top traders on the platform. The primary data source is: [Binance's Leaderboard](https://www.binance.com/en/futures-activity/leaderboard).

2. **Position Monitoring & Analysis**: Constantly checks for changes in positions of these top traders. If a change is detected, the system breaks down the data, analyzing the nature of the trade, such as:
    - Trading Pair (e.g., BTC/USDT)
    - Leverage Used
    - Trade Type (Short or Long)
    - Trader's identity
    - If it's a closing trade, whether it's winning or losing and by what percentage.

3. **Real-time Alerts**: Transforms the analyzed data into clear and concise trading signals which are sent out in real-time.

4. **Telegram Integration**: Utilizes the Telegram API to dispatch these trading alerts ensuring the client receives these notifications promptly.

## Benefits

- **Informed Decision Making**: By keeping tabs on top traders, clients can potentially use this information to guide their own trading strategies.
- **Promptness**: Through the Telegram API, alerts are delivered swiftly ensuring timely information dissemination.
- **Clarity**: Alerts are structured to provide all essential details without overwhelming the recipient, ensuring clarity and ease of understanding.