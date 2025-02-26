# NFT Pass Bot

Telegram бот для проверки наличия NFT и предоставления доступа к закрытому чату.

## Функционал

- Подключение TON кошелька через TonKeeper
- Проверка наличия NFT из определенной коллекции
- Автоматическая генерация одноразовых ссылок на закрытый чат
- Перенаправление на GetGems для покупки NFT

## Установка

1. Клонируйте репозиторий:
```bash
git clone https://github.com/your-username/nft-pass-bot.git
cd nft-pass-bot
```

2. Создайте виртуальное окружение:
```bash
python3 -m venv venv
source venv/bin/activate  # для Linux/MacOS
```

3. Установите зависимости:
```bash
pip3 install -r requirements.txt
```

4. Создайте файл .env и заполните его:
```env
BOT_TOKEN=ваш_токен_бота
PRIVATE_CHAT_ID=id_закрытого_чата
COLLECTION_ADDRESS=адрес_коллекции_nft
GETGEMS_URL=url_коллекции_на_getgems
MANIFEST_URL=url_манифеста
TON_API_KEY=ваш_ton_api_ключ
```

## Настройка

1. Создайте бота через @BotFather и получите токен
2. Создайте закрытую группу и добавьте бота администратором
3. Получите ID группы через @getidsbot
4. Загрузите манифест на GitHub Pages или другой хостинг
5. Получите API ключ на https://toncenter.com/

## Запуск

```bash
python3 pass_bot.py
```

## Деплой на Railway

1. Создайте аккаунт на Railway.app
2. Подключите GitHub репозиторий
3. Добавьте все переменные из .env в настройки проекта
4. Деплой произойдет автоматически

## Безопасность

- Не коммитьте файл .env в репозиторий
- Используйте одноразовые ссылки для приглашений
- Регулярно обновляйте зависимости

## Поддержка

При возникновении проблем создавайте Issue в репозитории.

# TON Connect Manifest

This repository hosts the manifest file for TON Connect integration.

## Files

- `tonconnect-manifest.json` - The manifest file for TON Connect
- `.nojekyll` - Prevents GitHub Pages from processing files through Jekyll 