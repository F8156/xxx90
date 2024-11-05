import ccxt
import pandas as pd
import matplotlib.pyplot as plt

# Initialize the exchange connection
exchange = ccxt.binance()  # Replace with your exchange of choice
symbol = 'BTC/USDT'

# Fetch historical OHLCV data (Open, High, Low, Close, Volume)
ohlcv = exchange.fetch_ohlcv(symbol, timeframe='1d', limit=100)
df = pd.DataFrame(ohlcv, columns=['Timestamp', 'Open', 'High', 'Low', 'Close', 'Volume'])
df['Timestamp'] = pd.to_datetime(df['Timestamp'], unit='ms')

# Plot closing prices
plt.figure(figsize=(12, 6))
plt.plot(df['Timestamp'], df['Close'], label='Closing Price')
plt.title(f'{symbol} Price Analysis')
plt.xlabel('Date')
plt.ylabel('Price (USDT)')
plt.grid()
plt.legend()
plt.show()

