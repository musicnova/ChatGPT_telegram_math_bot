# ChatGPT_math
Telegram bot with ChatGPT model by OpenAI (Example running here https://t.me/chatgpt_telegram_math_bot)


README: https://vc.ru/u/1389654-machine-learning/576592-instrukciya-kak-ispolzovat-chatgpt-s-python


How to deploy:
```
useradd -m tele1
sudo passwd tele1

sudo apt update
sudo apt -y install python3
sudo apt -y install python3.8
sudo apt -y install python3-pip

su - tele1
pip3 install virtualenv
virtualenv --version
```

How to run:

Clone repository:

```
git clone https://github.com/musicnova/telegram_math_bot.git
cd telegram_math_bot
git checkout day-2023-03-11
```

Create and activate environment:

```
echo python3 -m venv env
or
echo py -3.10 -m venv env
```

If you have Linux/macOS

```
echo source env/bin/activate
```

If you have windows

```
echo source env/scripts/activate
python3 -m pip install --upgrade pip
```

Install requirements in requirements.txt:

```
pip3 install -r requirements.txt
```

Create file '.env.prod' in main repository then provide API_KEY_CHATGPT and TG_BOT_TOKEN:

```
# in .env.prod file
API_KEY_CHATGPT=
TG_BOT_TOKEN=
DB_LINK=db.db
```

Run project:

```
API_KEY_CHATGPT=  TG_BOT_TOKEN=  python3 main.py
```
