# О веб-приложении

## Бизнес-требования (БТ) к приложению

1. Первичное наполнение БД тикеров публичных компаний. Необходимо учесть, что каждая компания может иметь несколько видов тикеров (привилегированные и обыкновенные акции).
2. Первичное наполнение БД о ценах на акции компании в определенный день проведения торгов начиная с 01.01.2020. (Цена открытия, Цена закрытия, Минимальная цена в этот день, Максимальная цена в этот день, Объем торгов).
3. Актуализация данных о ценах на акции определенной компании (или всех компаний) по требованию.
4. Построение табличного отчета о торгах за определенный промежуток времени для определенной компании.
5. Поиск компаний в реестре
6. Первоисточником данных о тикерах компаний и цен на акции должно служить API, предоставляемый биржей https://iss.moex.com/iss/reference/
7. Макет https://www.figma.com/file/Qg93mj7ivLgaI3xBZv9PaB/MOEXSync?node-id=0%3A1

## Требования к реализации

1. Отрисовка веб-приложения должна быть выполнена в браузере (выбор технологии свободный).
2. Должна быть настроена автоматическая миграция данных.
3. В качестве хранилища данных использовать легковесную встраиваимую СУБД SQLite.
4. Необходимо обеспечить построение архитектуры приложения с помощью паттерна MVC.
5. Должна быть предоставлена инструкция по развертыванию веб-приложения на виртуальной машине.

## Пожелания
1. Было бы здорово, чтобы были написаны тесты
2. Было бы здорово, чтобы была настроена система непрерывной интеграции https://travis-ci.com/ (хотя бы на сборку кода)