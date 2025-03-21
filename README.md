 # Дипломный Бот

Этот бот предназначен для автоматической генерации структуры и содержания дипломной работы на заданную тему. Бот использует GPT-4 для создания текста и сохраняет результат в форматах Markdown и Word (DOCX).

## Установка и настройка

1. **Клонируйте репозиторий:**
   ```bash
   git clone https://github.com/your-repo/diploma-bot.git
   cd diploma-bot
   ```

2. **Установите зависимости:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Настройте токен Telegram бота:**
   - Откройте файл `bot.py`.
   - Найдите строку:
     ```python
     bot = Bot(token="7722309470:AAF_WkaBZvK5iyS3kw0O2dpfLYrGLmG5o5k")
     ```
   - Замените `"7722309470:AAF_WkaBZvK5iyS3kw0O2dpfLYrGLmG5o5k"` на ваш токен Telegram бота.

4. **Настройте ID администратора:**
   - Найдите строку:
     ```python
     ADMIN_ID = 1404494933  # ID админа
     ```
   - Замените `1404494933` на ваш Telegram ID.

## Использование

1. **Запустите бота:**
   ```bash
   python bot.py
   ```

2. **Команды бота:**
   - `/start` - Начать работу с ботом.
   - `/generate_key` - Сгенерировать одноразовый ключ доступа (только для администратора).
   - `/get_file` - Получить текущую версию файла дипломной работы.

3. **Процесс работы:**
   - После запуска бота, введите код доступа (если требуется).
   - Введите тему дипломной работы.
   - Бот сгенерирует структуру работы и предложит начать генерацию содержания.
   - После завершения генерации, бот отправит вам файлы в форматах Markdown и Word.

## Зависимости

- `aiogram` - для работы с Telegram API.
- `g4f` - для взаимодействия с GPT-4.
- `python-docx` - для создания и редактирования Word документов.
- `uuid` - для генерации одноразовых ключей доступа.

## Лицензия

Этот проект распространяется под лицензией MIT. Подробности см. в файле [LICENSE](LICENSE).

## Автор

- **TETRIX_UNO**
- Telegram: [@TETRIX_UNO](https://t.me/TETRIX_UNO)

---

**Примечание:** Убедитесь, что у вас есть доступ к GPT-4 API и корректно настроены все зависимости перед запуском бота.
