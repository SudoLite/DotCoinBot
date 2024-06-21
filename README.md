[<img src="https://img.shields.io/badge/Telegram-%40Me-orange">](https://t.me/SudoLite)


![img1](.github/images/demo.png)

> 🇮🇷 README available in Persian [here](README-FA.md)

> Special Thanks [shamhi](https://github.com/shamhi)

## Functionality
| Functional                                                     | Supported |
|----------------------------------------------------------------|:---------:|
| Multithreading                                                 |     ✅     |
| Binding a proxy to a session                                   |     ✅     |
| Auto-purchase of items if you have coins (tap, attempts)       |     ✅     |
| Auto get all task if possible                                  |     ✅     |
| Random sleep time between clicks                               |     ✅     |
| Random number of clicks per request                            |     ✅     |
| Support tdata / pyrogram .session / telethon .session          |     ✅     |

## [Settings](https://github.com/SudoLite/DotCoinBot/blob/main/.env-example)
| Setup                      | Description                                                                |
|----------------------------|----------------------------------------------------------------------------|
| **API_ID / API_HASH**      | Platform data from which to launch a Telegram session (stock - Android)    |
| **AUTO_UPGRADE_TAP**       | Should I improve the tap _(True / False)_                                  |
| **MAX_TAP_LEVEL**          | Maximum level of tap pumping _(up to 15)_                                  |
| **AUTO_UPGRADE_ATTEMPTS**  | Should I improve the limit attempts _(True / False)_                       |
| **MAX_ATTEMPTS_LEVEL**     | Maximum level of limit attempts _(up to 15)_                               |
| **RANDOM_TAPS_COUNT**      | Random number of taps _(eg [50,200])_                                      |
| **SLEEP_BETWEEN_TAP**      | Random delay between taps in seconds _(eg [10,25])_                        |
| **USE_PROXY_FROM_FILE**    | Whether to use proxy from the `bot/config/proxies.txt` file (True / False) |

## Installation
You can download [**Repository**](https://github.com/SudoLite/DotCoinBot) by cloning it to your system and installing the necessary dependencies:
```shell
~ >>> git clone https://github.com/SudoLite/DotCoinBot.git
~ >>> cd DotCoinBot

# If you are using Telethon sessions, then clone the "converter" branch
~ >>> git clone https://github.com/SudoLite/DotCoinBot.git -b converter
~ >>> cd DotCoinBot

#Linux
~/DotCoinBot >>> python3 -m venv venv
~/DotCoinBot >>> source venv/bin/activate
~/DotCoinBot >>> pip3 install -r requirements.txt
~/DotCoinBot >>> cp .env-example .env
~/DotCoinBot >>> nano .env # Here you must specify your API_ID and API_HASH , the rest is taken by default
~/DotCoinBot >>> python3 main.py

#Windows
~/DotCoinBot >>> python -m venv venv
~/DotCoinBot >>> venv\Scripts\activate
~/DotCoinBot >>> pip install -r requirements.txt
~/DotCoinBot >>> copy .env-example .env
~/DotCoinBot >>> # Specify your API_ID and API_HASH, the rest is taken by default
~/DotCoinBot >>> python main.py
```

Also for quick launch you can use arguments, for example:
```shell
~/DotCoinBot >>> python3 main.py --action (1/2)
# Or
~/DotCoinBot >>> python3 main.py -a (1/2)

#1 - Create session
#2 - Run clicker
```
