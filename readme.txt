﻿Лэндинг для компании Maripo.

Эффект при нажатии на надпись MARIPO (содержимое папки code_by_codrops_com) via https://github.com/codrops/LetterInteractions/

===============

ИНСТРУКЦИЯ ПО РЕДАКТИРОВАНИЮ КОНТЕНТА

Оба файла, предназначенных для редактирования контента, можно открыть и изменить через блокнот или любой другой текстовый редактор.
При сохранении изменений в файлах рекомендуется убедиться в корректном выборе кодировки (UTF-8).


1. Редактирование содержимого подразделов сайта.

HTML-содержимое подразделов представлено файлом links.js


Соответствия меток и разделов:

delivery - Оплата и Доставка
contacts - Контакты
produce - Производство
bonus - Бонусная программа
about - О нас
style - Стиль Maripo
wholesale - Оптовым клиентам
refund - Обмен и возврат
sizes - Соответствие разделов
care - Уход за одеждой

Для редактирования содержания этих страниц необходимо заменить текст в кавычках после двоеточия на нужный HTML-код, сохраняя при этом синтаксис ("метка": "HTML-код").

При использовании двойных кавычек внутри блока с HTML-кодом необходимо ставить перед каждой из них обратный слэш("метка": "\"текст в кавычках\"").


2. Редактирование представленного товара.

Каталог товаров представлен файлом gallery.js


Синтаксис и соответствие меток:

    {"title": "наименование товара",
     "price": "цена (см. примечание N1)"
     "description": "описание товара",
     "sizes": "размеры",
     "consist": "состав",
     "colour": "цвета",
    "images": [
        "ссылка на изображение 1",
        "ссылка на изображение 2 (и т.д. - см. примечание N2)"]}
        
Примечание N1:
    В поле "Цена" следует указать только число, значок рубля будет подставлен автоматически. Если оно представлено только цифрами(то есть, не в виде значения типа "1000-2000"), можно - и даже желательно - указать его без кавычек ("price": цена).

Примечание N2:
    Оригинал изображения должен находиться в папке /products/. Миниатюра изображения должна иметь такое же название, быть по размеру не менее 290*290 пикселей и находиться в папке /products/min/.

Синтаксическая модель, используемая в этих таблицах данных, называется JSON. При подозрении, что в ходе изменения файла где-то была допущена синтаксическая ошибка, можно проверить это с помощью онлайн-валидаторов, таких, как, например, https://jsonlint.com/