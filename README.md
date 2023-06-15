# GyverHub-projects
Это база проектов на [платформе GyverHub](https://github.com/GyverLibs/GyverHub)
- Можно добавлять свои проекты в базу http://hub.gyver.ru/projects/
- Встроенный в GyverHub механизм обновления подскажет юзеру, что проект обновился
- По согласию юзера обновление само скачается с гитхаба проекта и установится

### Как добавить свой проект
#### Сделать репозиторий
- Зарегистрироваться на GitHub, создать репозиторий проекта (см. гугл)
- Загрузить бинарник проекта, он должен находиться по пути `/bin/firmware.bin`
- Создать и заполнить файл информации о проекте, он должен находиться по пути `/project.json`

#### Файл информации
Образец файла информации:
```json
{
  "version": "x.x",
  "notes": "комментарии к версии обновления",
  "about": "Короткое описание проекта"
}
```

- При изменении кода версии проекта платформа GyverHub предложит юзеру обновиться
- Название проекта будет взято из названия репозитория

#### Добавление в базу
Нужно просто сделать fork данного репозитория, добавить ссылку на репозиторий своего проекта в файл projects.txt и создать Pull request:
- Перейти на [страницу редактирования](https://github.com/GyverLibs/GyverHub-projects/edit/main/projects.txt) файла projects.txt
    - Если это первое добавление - нажать **Fork this repository**
- Добавить ссылку на репозиторий своего проекта в список проектов
- Нажать **Commit changes...** в правом верхнем углу экрана
- Нажать **Propose changes** в появившемся окне
- Нажать **Create pull request** в правом верхнем углу экрана
- Нажать **Create pull request** на открывшейся странице
- Ждать когда я приму изменения =)
