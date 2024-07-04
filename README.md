# CryptoTelegramWalletBot
CryptoTelegramWalletBot is a Telegram bot designed to manage cryptocurrency assets. It offers real-time tracking, chart generation, and reporting capabilities. Users can also enable volatility alerts to be notified of significant price fluctuations in their assets. The bot retrieves financial data via the Binance API.

## Requirements
CryptoTelegramWalletBot is tailored for individual use. It requires a hosting platform (the developer uses a Raspberry Pi) and API keys for both a Telegram Bot and a Binance account. You can find a guide to obtaining Binance API keys here, and instructions for creating a Telegram bot and acquiring its API token here.

Due to its design for personal or small group use, the bot may experience noticeable delays if it receives too many simultaneous requests. This could lead to unexpected results.

The bot's code has been verified on Python 3.9.5. Below is a list of necessary dependencies, which you can install using the following commands:
```
pip install python-telegram-bot 
pip install python-binance 
pip install mplfinance
pip install numpy
pip install pandas
```
Note: If you're running this program on a Raspberry Pi, ensure that you have Python 3 installed to avoid defaulting to Python 2.7.x.
