Описание проекта:
Проект API Yatube - это API для социальной сети Yatube.

С помощью API Yatube можно запрашивать данные о постах зарегестрированных пользователей, группах, комментариях к постам, а также создавать новые посты  в социальной сети Yatube.

Yatube - это учебный проект курса "Python-разработчик" от Яндекс-Практикума, который представляет собой социальную сеть.

Автор: Влад Буганов

Как запустить проект:
Клонировать репозиторий. 

Список команд для командной строки
git clone https://github.com/VladislavRZN/api_final_yatube.git
cd api_final_yatube

Cоздать и активировать виртуальное окружение:
# Команды для Windows:
python -m venv venv
source venv/Scripts/activate

# Команды для Linux и macOS:
python3 -m venv venv
source venv/bin/activate

Установить зависимости из файла requirements.txt:
python -m pip install --upgrade pip
pip install -r requirements.txt

Выполнить миграции:
python manage.py migrate

Запустить проект на локальном сервере:
python3 manage.py runserver

Примеры запросов к API:
Получить список всех постов (GET):
http://127.0.0.1:8000/api/v1/posts/
Получить определенный пост (GET):

http://127.0.0.1:8000/api/v1/posts/1/
Получить коментарии определенного поста (GET):

http://127.0.0.1:8000/api/v1/posts/1/comments/
Получить список всех групп (GET):

http://127.0.0.1:8000/api/v1/groups/
Создать новый пост (POST):

(Требуется аутентификация)

http://127.0.0.1:8000/api/v1/posts/
