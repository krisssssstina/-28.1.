Финальный тестовый проект Skillfactory курса INTQAP

Автоматизированное ui-тестирование нового интерфейса авторизации в личном кабинете от заказчика Ростелеком Информационные Технологии (https://b2c.passport.rt.ru/)

Тест-кейсы доступны по ссылке: https://docs.google.com/spreadsheets/d/1NyvLB8QG6hJnE3ic3-jKHmbhRKP6O3S4SA5u0WXcUqg/edit?usp=sharing

Баг-репорты доступны по ссылке: https://docs.google.com/spreadsheets/d/15a4L9QbWwTx2gtWUfiQONTaLG6DXJ028VMpsLEd-3P8/edit?usp=sharing

В папке pages в файле base_page.py находится конструктор webdriver и общие для всех тестируемых страниц методы.

В папке pages в файлах auth_page.py, change_pass_page.py, reg_page.py находятся методы проверок: файл auth_page.py содержит методы проверок формы авторизации; файл change_pass_page.py содержит методы проверок формы восстановления пароля; файл reg_page.py содержит методы проверок формы регистрации.

В папке tests в файлах test_auth_page.py, test_change_pass_page.py, test_reg_page.py находятся тесты. Все тесты помечены номером, совпадающим с номером тест-кейса в файле: https://docs.google.com/spreadsheets/d/1NyvLB8QG6hJnE3ic3-jKHmbhRKP6O3S4SA5u0WXcUqg/edit?usp=sharing. Во всех файлах с тестами, находятся закомментированные команды для запуска тестов из командной строки (запуск тестов формы авторизации: # python -m pytest -v --tb=line tests/test_auth_page.py; запуск тестов формы восстановления пароля: # python -m pytest -v --tb=line tests/ test_change_pass_page.py; запуск тестов формы регистрации: # python -m pytest -v --tb=line tests/ test_reg_page.py)

В папке pages в файле "locators.py находятся все локаторы.

В корне проекта в файле conftest.py находится фикстура с функцией открытия и закрытия браузера.

В корне проекта в файле settings.py находятся методы и переменные для параметризации тестов

В корне проекта в файле pytest.ini зарегистрированы метки маркировок тестов.

В корне проекта в файле requirements.py описаны используемые библиотеки.
