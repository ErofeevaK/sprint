# <span style="color:MediumPurple">Автоматизированные тесты для Stellar Burgers</span> 

Этот проект содержит комплекс автоматизированных тестов для веб-сервиса Stellar Burgers, включая проверку функционала регистрации, авторизации, навигации и конструктора бургеров.

## Требования
- Python 3.8+
- Браузер Chrome
- Selenium WebDriver

## Необходимо проверить

### Регистрация
- Успешная регистрация:
  - Поле «Имя» не пустое
  - Email в корректном формате (логин@домен)
  - Пароль не менее 6 символов
- Ошибка при некорректном пароле

### Вход 
- Через кнопку «Войти в аккаунт» на главной
- Через кнопку «Личный кабинет»
- Через кнопку в форме регистрации
- Через кнопку в форме восстановления пароля

### Переходы
- В личный кабинет по клику на «Личный кабинет»
- Из личного кабинета:
  - В конструктор по клику на «Конструктор»
  - На главную по клику на логотип Stellar Burgers
  
### Выход из аккаунта
- По кнопке «Выйти» в личном кабинете

### Раздел конструктор
- Переходы между разделами:
  - «Булки»
  - «Соусы»
  - «Начинки»

## Установка

1. Клонируйте репозиторий
2. Установите зависимости: `pip install -r requirements.txt`
3. Запустите тесты: `pytest tests/`

## Структура тестов
- `test_registration.py`: Тесты регистрации пользователя
- `test_login.py`: Тесты входа в систему
- `test_navigation.py`: Тесты навигации между страницами
- `test_logout.py`: Тесты выхода из системы
- `test_constructor.py`: Тесты разделов конструктора бургеров
 
 
