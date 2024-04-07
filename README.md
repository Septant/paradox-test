<p align="center">
  <a href="https://angular.io" target="blank"> <img src="https://angular.io/assets/images/logos/angular/angular.svg" width="200" alt="Angular logo"> </a>
</p>

# Frontend

Тестовое задание для Парадокс <br>
Node version 18.10.0 <br>
Версия Angular: [Angular CLI](https://github.com/angular/angular-cli) version 16.2.10.

### Сторонние ресурсы
В проекте используются [moment.js](https://momentjs.com/) и [Taiga-ui](https://taiga-ui.dev)

### Режим разработки

`ng serve`: Запуск в режиме разработчика. Рабочий порт: `http://localhost:4200/`. 

### Сборка 

`ng build`: Сборка проекта. Артефакты собираются в папке `dist/`. Содержимое папки dist/frontend необходимо скопировать в `dist` backend под именем `client` после сборки backend-проекта.

# Модули

## 1. Теги

Облако тегов, с возможностью добавления, а также редактирования/удаления для неиспользующихся тегов. <br>
Клик по `+` добавляет новую плашку тега, нажатие `Enter` после заполнения добавляет новый тег. <br>
Для редактирования дважды кликните тегу. <br>
Удаление по нажатию на иконку крестика тега.

## 2. Уведомления

Сетка карточек уведомлений с просмотром ранее созданных и созданием новых (с указанием содержания и срока выполнения). <br>
Для пометки уведомления как выполненного кликнитне на чекбокс. <br>
Форма создания нового уведомления доступна по клику на карточку `+`.

## 3. Заметки
Таблица заметок с функционалом добавления, просмотра, редактирования и удаления заметок. <br>
Переход на заметку осуществляется по двойному клику строки. <br>
Редактирование и удаление доступны по кнопкам столбца "действия". <br>
Создание - отдельная кнопка слева над таблицей. <br>

# Структура:
1. [api-services](/src/app/api-services): абстракции над HttpClient и конечные endpoint'ы, перехватчики
2. [outer-wrap](/src/app/outer-wrap): footer и header 
3. [models](/src/app/models): интерфейсы
4. Модули:
   * [tabs](/src/app/tabs): tab-панель навигации по модулям приложения
   * [notes](/src/app/notes): модуль заметок
   * [notifications](/src/app/notifications): модуль уведомлений
   * [tags](/src/app/tags): модуль тегов
5. app.* - корень приложения


