# 🚀 Monad Wallet Manager

**Monad Wallet Manager** – это инструмент для управления EVM-кошельками, который позволяет:
- Загружать приватные ключи из файла
- Добавлять кошельки в базу данных
- Назначать прокси
- Проверять баланс кошельков
- Запускать автоматические и ручные маршруты
- Покупать токены MON на всех кошельках

---

## ⚙️ Installation

### 1️⃣ Clone repository:
```bash
git clone https://github.com/florzoye/monad_automatic.git
```

### 2️⃣ Go to folder 📂:
```bash
cd monad_automatic
```

### 3️⃣ Install requirements:
```bash
pip install -r requirements.txt
```

---

## 📌 Features
- **Добавление кошельков** из CSV, Python-списка или файла приватных ключей
- **Назначение прокси** из `proxy.txt`
- **Проверка баланса** кошельков
- **Автоматический маршрут** (запускает скрипты в порядке их последнего выполнения)
- **Ручной маршрут** (возможность выбрать последовательность скриптов)
- **Покупка MON** на всех кошельках

---

## 🚀 Usage

### 🏗️ Запуск основного скрипта:
```bash
python main.py
```

### 🛠️ Доступные команды:
| №  | Действие |
|----|----------|
| 1️⃣  | Использовать готовые кошельки |
| 2️⃣  | Создать новые кошельки |
| 3️⃣  | Удалить все кошельки из базы |
| 4️⃣  | Запустить автоматический маршрут |
| 5️⃣  | Выбрать ручной маршрут |
| 6️⃣  | Добавить прокси к кошелькам |
| 7️⃣  | Вывести все адреса кошельков |
| 8️⃣  | Купить $MON на все кошельки |
| 9️⃣  | Выйти |
| 🔟  | Загрузить приватные ключи из `private_key.txt` |

---

## 📥 Loading Private Keys
Добавьте приватные ключи в `private_key.txt` **(по одному в каждой строке)** и выполните команду:
```bash
python main.py
```
Выберите опцию **(10) Загрузить приватные ключи из private_key.txt**, и все ключи автоматически добавятся в базу.

---

## 🔧 Configuration
Настройки RPC и другие параметры можно изменить в файле `config.py`:
```python
monad_rpc = 'https://testnet-rpc.monad.xyz/'
arb_rpc = "https://1rpc.io/arb"
wallets = [{'key': '123qweasxd','proxy': 'user:pass@ip:port'}]
```

---

## 🤝 Contributing
Pull requests приветствуются! Если у вас есть идеи по улучшению, создавайте issue или форкните репозиторий. 🚀

---

## 📜 License
Этот проект распространяется под лицензией MIT. Используйте на свой страх и риск.

