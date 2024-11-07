# DisordTokenSorterBD

## English Version

### Overview
This program sorts tokens based on different criteria including year, month, and optionally day. The sorted tokens are organized into output directories for easier analysis.

### Features
- Sort tokens by year, month, and optionally by day.
- Additional sorting by relative time (years and months since creation).
- Tracks failed attempts to decode tokens.
- Progress output to track processing completion percentage.

### Prerequisites
- Python 3.x
- File `tokens.txt` containing one token per line.

### Usage
1. Place all tokens into a file named `tokens.txt`, where each token is on a new line.
2. Run the script by executing:
   ```
   python script.py
   ```
3. You will be prompted to decide if you want to sort by day:
   - Enter "y" for yes or "n" for no.

### Output
- The output is stored in the `output/` directory with a timestamped folder name.
- The tokens are sorted in different subdirectories based on the selected criteria (year, month, day, relative time).

### Example
After running the script, the output directory may contain:
- `sorted_by_year/` - Contains files like `2021.txt`, `2022.txt`, etc.
- `sorted_by_month/` - Contains files like `2021-05.txt` for tokens created in May 2021.
- `sorted_by_day/` (if selected) - Contains files like `2021-05-15.txt` for tokens created on May 15, 2021.
- `sorted_by_relative_time_year/` - Contains files named like `2 year(s).txt` for tokens created 2 years ago.
- `sorted_by_relative_time_month/` - Contains files for tokens sorted by both years and months since creation.
- `failed.txt` - Contains any tokens that could not be processed.

### Notes
- Tokens must be in `tokens.txt` in the proper format.
- Ensure all required dependencies are installed.

### License
Feel free to modify and use this script as needed.

---

## Русская версия

### Обзор
Эта программа сортирует токены по различным критериям, включая год, месяц и по желанию день. Сортированные токены сохраняются в выходные папки для удобного анализа.

### Функции
- Сортировка токенов по годам, месяцам и при желании по дням.
- Дополнительная сортировка по относительному времени (года и месяцы с момента создания).
- Запись неудачных попыток расшифровать токены.
- Вывод прогресса поцентной завершенности.

### Пререквизиты
- Python 3.x
- Файл `tokens.txt`, содержащий один токен на каждой линии.

### Использование
1. Поместите все токены в файл `tokens.txt`, где каждый токен на отдельной строке.
2. Запустите скрипт командой:
   ```
   python script.py
   ```
3. Вам будет предложено выбрать, сортировать ли по дням:
   - Введите "y" для да или "n" для нет.

### Вывод
- Все результаты сохраняются в папке `output/` с именем, содержащим время запуска.
- Токены сортируются в различные папки в зависимости от выбранных критериев (год, месяц, день, относительное время).

### Пример
После запуска скрипта папка `output` может содержать следующие подпапки:
- `sorted_by_year/` - содержит файлы такие, как `2021.txt`, `2022.txt` и т.д.
- `sorted_by_month/` - файлы, например, `2021-05.txt` для токенов, созданных в мае 2021 года.
- `sorted_by_day/` (если было выбрано) - файлы, например, `2021-05-15.txt` для токенов, созданных 15 мая 2021 года.
- `sorted_by_relative_time_year/` - файлы, такие как `2 year(s).txt` для токенов, созданных 2 года назад.
- `sorted_by_relative_time_month/` - файлы для токенов, сортированных по годам и месяцам с момента создания.
- `failed.txt` - содержит токены, которые не удалось обработать.

### Заметки
- Токены должны находиться в `tokens.txt` в правильном формате.
- Убедитесь, что все необходимые зависимости установлены.

### Лицензия
Вы можете изменять и использовать этот скрипт по собственному усмотрению.
