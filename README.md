# Swift backup RU
Авто-бекапер для линукса с отчетностью по почте. Тестировался на Debian 8 Jessie.

### Что бекапит?
Позволяет бэкапить файлы и БД MySQL.
### Где хранит?
Все данные будут хранится на локальном хранилище, и на удаленном FTP сервере.
### Когда узнаю об этом?
На почту будет приходить 2 письма:
 * Первое письмо - короткий отчет. Просто показывает размеры итоговых файлов
 * Второе письмо - полный отчет. Содержит всю процедуру бекапа.

# Настройка

Все настройки можно найти в `backup.sh`
Этот файл и надо запускать в кроне.

После настройки файла надо установить эти пакеты: `lftp`, `ssmtp` and `uuenview`.
## ssmtp
Подключите `ssmtp` к любому SMTP серверу типа `gmail` или `yandex`, чтобы отправлять письма было просто.
Вот тут можно найти как его настроить: http://serveradministrator.ru/mail/ssmtp/
