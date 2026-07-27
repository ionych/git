# 📌 git

Git — это система контроля версий, доступная на каждом компьютере разработчика. Она позволяет легко создавать ветки и сливать изменения. GitHub делает Git ещё удобнее для индивидуальной и командной работы 🤝

Здесь я делюсь командами Git, которые использовал для создания своего портфолио на GitHub.

## Навигация

- [Создание, клонирование, push и pull репозиториев](#task-1)
- [Создание и добавление удалённых репозиториев](#task-2)
- [Создание веток и слияние](#task-3)

## Task 1

##### Создание, клонирование, push и pull репозиториев
```git
git init ionov_agency                                         # Создать репозиторий для Flask-проекта
git clone git@github.com:ionych/ionych.git                   # Клонировать свой репозиторий
git clone git@github.com:testrusau/testrusau.git             # Клонировать внешний репозиторий для изучения
cd testrusau                                                 # Отправить данные из внешнего репозитория в свой
git push git@github.com:ionych/testrusau.git main:main
git add README.md                                            # Редактировать README.md и закоммитить изменения
git commit -m "Обновил README: добавил описание проекта"
git push

```
## Task 2

##### Создание и добавление удалённых репозиториев

```git
git init ionov_agency                                        # Инициализировать локальный репозиторий
git branch -m main                                           # Переименовать ветку в main
git add .                                                    # Добавить все файлы
git commit -m "First commit: Flask-приложение для рекламного агентства"  # Первый коммит
git remote add origin https://github.com/ionych/ionov_agency.git  # Привязать удалённый репозиторий
git remote -v                                                # Проверить привязку
git push -u origin main                                      # Отправить на GitHub

git add README.md                                            # Обновить README с описанием проекта
git commit -m "Добавил README с описанием проекта и QA-артефактами"
git push

git add schema.sql data.sql                                  # Добавить SQL-скрипты для базы данных
git commit -m "Добавил SQL-скрипты schema.sql и data.sql"
git push
```