# Binance Futures Testnet Trading Bot

##  Overview
This is a simple Python CLI-based trading bot that places MARKET and LIMIT orders on Binance Futures Testnet.

##  Setup

1. Clone the repo:
   git clone <your-repo-link>
   cd trading_bot

2. Install dependencies:
   pip install -r requirements.txt

3. Set environment variables:
   export BINANCE_API_KEY=your_key
   export BINANCE_API_SECRET=your_secret

4. Run the bot:

### MARKET Order:
python cli.py --symbol BTCUSDT --side BUY --type MARKET --quantity 0.001

### LIMIT Order:
python cli.py --symbol BTCUSDT --side SELL --type LIMIT --quantity 0.001 --price 60000

## Features
- MARKET and LIMIT orders
- BUY / SELL support
- CLI input validation
- Logging to bot.log
- Error handling

## Project Structure
- bot/client.py → API client
- bot/orders.py → order execution
- bot/validators.py → input validation
- bot/logging_config.py → logging setup
- cli.py → CLI entry point

## Logs
All logs are stored in:
bot.log

##  Assumptions
- Binance Futures Testnet account is already created
- API keys are valid