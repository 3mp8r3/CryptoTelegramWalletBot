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

Starting Up the CryptoTelegramWalletBot
After installing the dependencies and obtaining the three API keys, you'll need to make these keys accessible to the bot. This ensures proper connection setup with Binance and Telegram. To do this, format the data/api_keys.txt file as follows (note that depending on the current state of this GitHub repository, you may need to create the api_keys.txt file):
```
telegram_bot_token
binance_api_public_key
binance_api_private_key
```
With that in place, you're ready to go! Simply execute the main.py script with Python.

Upon successful launch of the bot, you should see the following confirmation messages:
```
>> [Current Date and Time]-BOT: Loading Telegram bot: SUCCESS
>> [Current Date and Time]-BOT: Loading Binance Client: SUCCESS
>> [Current Date and Time]-BOT: Callbacks initialized. Polling started
```

## Usage
Once the  bot is up and running, the main menu will always be available at the `/home` commmand:

![Home Menu](https://github.com/3mp8r3/CryptoTelegramWalletBot/blob/main/menu_README.png)

Key Features of the CryptoTelegramWalletBot
•  ** Set Wallet**: Users can input their cryptocurrency holdings, specifying the quantity and purchase price. The bot uses this data to calculate and track profits or losses based on live market prices.

•  ** My Wallet**: This feature provides a detailed wallet report and visualizes the performance of the user's crypto assets over various time frames.

•  ** Check Asset**: Offers a chart display for any cryptocurrency, across all time scales available on Binance. To see the full range of supported queries, refer to the ** Help** command. Note: This function is available even without setting up a wallet.

•  bell Notifications: Enables users to receive daily wallet summaries and price volatility alerts for rapid increases or decreases in the value of their stored assets.

Please check the "🚁Help" button or type `/help` in the chat to get informations live from the bot.
