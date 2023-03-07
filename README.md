# Skillfactory_final_project

Финальный тестовый проект Skillfactory курса Тестировщик-автоматизатор на Python (QAP)

Автоматизированное тестирование нового UI авторизации в личном кабинете от заказчика Ростелеком Информационные Технологии (https://b2c.passport.rt.ru/)
____

Тест кейсы и баг репорты доступны по ссылке: https://docs.google.com/spreadsheets/d/1scYGrSIgPVQXkA1bd2Z0y8y5KEKGz4Q5mpZxz_hFlk0/edit?usp=sharing

1. Папка pages: в файле base_page.py находится конструктор webdriver и общие для всех тестируемых страниц методы.

2. Папка pages: в файлах auth_page.py, change_pass_page.py, reg_page.py находятся методы проверок: файл auth_page.py содержит методы проверок формы авторизации; файл change_pass_page.py содержит методы проверок формы восстановления пароля; файл reg_page.py содержит методы проверок формы регистрации.

3. Папка tests: в файлах test_auth_page.py, test_change_pass_page.py, test_reg_page.py находятся тесты. Все тесты помечены номером, совпадающим с номерами тест кейсов. 

4. Папка pages: в файле "locators.py находятся все локаторы.

5. В файле conftest.py находится фикстура с функцией открытия и закрытия браузера. 

6. В файле settings.py находятся методы и переменные для параметризации тестов

7. В файле pytest.ini зарегистрированы метки маркировок тестов.

8. В файле requirements.py описаны используемые библиотеки.

Инструкция: 
1. "pip install -r requirements.txt" - установка зависимостей.
2. "python -m pytest -v —tb=line tests/test_auth_page.py" - запуск тестов формы авторизации.
3. "python -m pytest -v —tb=line tests/ test_change_pass_page.py" - запуск тестов формы восстановления пароля.
4. "python -m pytest -v —tb=line tests/ test_reg_page.py" - запуск тестов формы регистрации.
