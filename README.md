# Log Archiver

This project provides a simple script to archive logs from a specified directory. The logs are compressed into a `.tar.gz` archive and stored in a designated location. The original files are then deleted after the successful creation of the archive.

## Description
The script takes a directory path containing log files as an argument, creates a compressed archive of the logs, and saves it with a timestamp. After the archive is successfully created, the original log files in the provided directory are deleted to free up space.

## Features
- Takes a directory path as an argument.
- Compresses the logs into a `.tar.gz` archive.
- Saves the archive in the home directory.
- Deletes the original log files after successful compression.
- Logs the date and time of the archive operation.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/DragonVV/log-archiver.git

    Navigate to the project directory:

cd log-archiver

Make the script executable:

    chmod +x log_archiver.sh

Usage

To archive logs from a specified directory, run the script with the directory path as an argument:

log-archive /path/to/logs

For example, to archive logs from /var/log:

log-archive /var/log

How it Works

    The script takes the directory path (/path/to/logs) as an argument.

    It creates a timestamped .tar.gz archive of the contents of the specified directory.

    After successfully creating the archive, it verifies that the archive is not empty.

    Once the archive is confirmed to be valid, the original log files in the directory are deleted.

    The script logs the date and time of the operation to a log file.

License

This project is licensed under the MIT License.


This explanation covers:
- What the script does.
- How to install and use it.
- A brief explanation of the script's logic.


# Log Archiver

Этот проект представляет собой простой скрипт для архивирования логов из указанной директории. Логи сжимаются в архив формата `.tar.gz` и сохраняются в выбранном месте. После успешного создания архива оригинальные файлы удаляются.

## Описание
Скрипт принимает путь к директории с логами в качестве аргумента, создает сжатый архив с логами и сохраняет его с временной меткой. После успешного создания архива оригинальные файлы логов в указанной директории удаляются для освобождения места.

## Особенности
- Принимает путь к директории как аргумент.
- Сжимает логи в архив `.tar.gz`.
- Сохраняет архив в домашней директории.
- Удаляет оригинальные файлы логов после успешной архивации.
- Логирует дату и время операции архивации.

## Установка
1. Клонируйте репозиторий:
   ```bash
   git clone https://github.com/DragonVV/log-archiver.git

    Перейдите в директорию проекта:

cd log-archiver

Сделайте скрипт исполняемым:

chmod +x log_archiver.sh

Переместите скрипт в /usr/local/bin/ для удобства запуска:

sudo mv log_archiver.sh /usr/local/bin/log-archive

Использование

Чтобы архивировать логи из указанной директории, выполните скрипт с путём к директории в качестве аргумента:

log-archive /path/to/logs

Например, чтобы архивировать логи из /var/log:

log-archive /var/log

Как это работает

    Скрипт принимает путь к директории (/path/to/logs) как аргумент.

    Он создает сжатый архив .tar.gz из содержимого указанной директории.

    После успешного создания архива проверяется, что архив не пустой.

    Если архив создан успешно, оригинальные файлы логов в директории удаляются.

    Скрипт логирует дату и время операции в лог-файл.

Лицензия

Этот проект распространяется под лицензией MIT.

https://roadmap.sh/projects/log-archive-tool
