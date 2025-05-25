Telegram Crypto Analysis Bot

A Telegram bot that provides technical analysis for cryptocurrencies, including RSI scans, asset bias scoring, and MACD/RSI divergence detection. It fetches market data from CoinGecko and OHLCV data from a specified cryptocurrency exchange (default: Gate.io) using the ccxt library, and performs technical analysis using the pandas_ta library.

Features





/start: Displays a welcome message and shows available commands.



/help: Lists all commands with descriptions.



/rsi: Scans the top ~100 coins (configurable) for overbought (>70) or oversold (<30) RSI conditions across multiple timeframes (5m, 15m, 1h, 4h, 1d).



/analyze [SYMBOL]: Analyzes a specific trading pair (e.g., BTC/USDT) for bullish/bearish bias based on technical indicators (MACD, RSI, moving averages, trends, volume, candlestick patterns) across multiple timeframes, with BTC/ETH market context.



/bias: Identifies the top 10 tokens likely to go up or down from a predefined list, based on technical analysis scores.



/macd_divergences: Detects bullish and bearish (classic and hidden) MACD divergences in the last 6 candles for a predefined token list.



/rsi_divergences: Detects bullish and bearish (classic and hidden) RSI divergences in the last 6 candles for a predefined token list.

Requirements





Python 3.8+



Telegram Bot Token (obtain from BotFather)



Libraries: python-telegram-bot, ccxt, pandas, pandas_ta, numpy<1.25, nest_asyncio, requests
