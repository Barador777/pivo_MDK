<p align="center">
  <!-- Можешь вставить сюда свой баннер/скриншот главного окна -->
  <img width="1000" height="431" alt="Пиво Banner" src="https://disk.yandex.ru/client/disk?source=main-loginmenu&idApp=client&dialog=slider&idDialog=%2Fdisk%2F%7B4331EF29-0F41-407C-A991-94BA66835733%7D.png" />
</p>

<h1 align="center">Каталог пива / Пивной магазин</h1>

<p align="center">
  <a href="#">
    <img src="https://img.shields.io/badge/Version-v3.0-brightgreen.svg?style=flat-square" alt="Version" />
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/C%23-.NET%20Framework-purple.svg?style=flat-square" alt="C#" />
  </a>
  <a href="#">
    <img src="https://shields.io](https://img.shields.io/badge/Windows-Forms-blue.svg?style=flat-square)" alt="Windows Forms" />
  </a>
  <a href="#">
    <img src="https://shields.io](https://img.shields.io/badge/Database-MS%20Access-red.svg?style=flat-square)" alt="Access" />
  </a>
  <a href="LICENSE">
    <img src="https://shields.io" alt="License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)" />
  </a>
</p>

# Приложение «Пиво» на Windows Forms + MS Access

Учебный проект: десктопное приложение для учёта, поиска и просмотра каталога пива с разграничением прав доступа (авторизация и регистрация пользователей).

## What can it do?

## Screenshots

### Главное окно и каталог
<p align="center">
  <!-- Замени ссылку на свой скриншот Form1 -->
  <img width="1000" height="756" alt="Главное окно" src="https://disk.yandex.ru/client/disk?source=main-loginmenu&idApp=client&dialog=slider&idDialog=%2Fdisk%2F%7B57F575A5-9CEE-4D78-A717-93C525FC74FD%7D.png" />
</p>

### Карточка товара и добавление записи
<p align="center">
  <!-- Замени ссылку на свой скриншот BeerDetailForm / AddForm -->
  <img width="632" height="608" alt="Карточка пива" src="https://disk.yandex.ru/client/disk?source=main-loginmenu&idApp=client&dialog=slider&idDialog=%2Fdisk%2F%7B1F6CC40B-FA3A-40DC-9896-D0CEC3A61C68%7D.png" />
</p>

### 🍺 Основной функционал
- **Авторизация и регистрация**: вход в систему через `LoginForm` и создание нового аккаунта в `RegisterForm`.
- **Просмотр каталога**: удобная таблица со всем ассортиментом на главном экране (`Form1`).
- **Детальная карточка (`BeerDetailForm`)**: просмотр подробной информации о выбранном сорте пива.
- **Поиск и фильтрация (`SearchForm`)**: быстрый поиск позиций по параметрам и характеристикам.
- **Управление ассортиментом (`AddForm`)**: добавление новых позиций в базу данных.

## Usage

1. **Запуск**: открываешь `пиво.slnx` в Visual Studio (сборка под `x64` или `Any CPU`), жмёшь `F5`.
2. **Авторизация**: вводишь логин и пароль в окне входа или регистрируешь нового пользователя.
3. **Просмотр и поиск**: изучаешь каталог в главном окне, открываешь подробную карточку товара или пользуешься формой поиска.
4. **Редактирование**: добавляешь новые позиции через форму добавления.

## Installation

1. Клонируй репозиторий:
```bash
git clone https://github.com
```
2. Открой решение `пиво VS 2.0/пиво/пиво.slnx` в Visual Studio.
3. Убедись, что файл базы данных `баратрум.accdb` находится в директории проекта и в выходной папке (`bin/Debug` или `bin/x64/Debug`).
4. Нажми `F5` для запуска.

## Test Accounts

| Логин | Пароль | Роль / Доступ |
|-------|--------|---------------|
| admin | 123    | Администратор |
| user  | 123    | Пользователь  |

*(Замени данные в таблице на реальные логины и пароли из твоей таблицы пользователей в `баратрум.accdb`)*

## Functionality & Libraries

- **C# / .NET Framework 4.7.2** — язык и целевая платформа
- **Windows Forms** — графический интерфейс пользователя
- **MS Access (`баратрум.accdb`) + OleDb** — локальная реляционная база данных
- **Typed DataSet (`баратрумDataSet`) / BindingSource** — привязка и фильтрация данных

## Implementation Notes

- Проект скомпилирован с поддержкой архитектуры **x64** (важно для корректной работы драйвера `Microsoft.ACE.OLEDB` при подключении к `.accdb`).
- Работа с данными организована через типизированные датасеты (`баратрумDataSet` и `баратрумDataSet1`).
- Интерфейс разделён на логические модули: авторизация (`LoginForm`), регистрация (`RegisterForm`), главный каталог (`Form1`), детальный просмотр (`BeerDetailForm`), поиск (`SearchForm`) и добавление (`AddForm`).

## Useful Links

- [Microsoft Access](https://microsoft.com) — СУБД
- [Windows Forms](https://microsoft.com) — документация
- [ADO.NET / OleDb](https://microsoft.com) — работа с Access

## Acknowledgments & Mission

Огромная благодарность моему преподавателю за то, что заставил сделать это по всем правилам проектирования, а не «как получится». 

И спасибо Microsoft за то, что Access до сих пор существует. Он странный, но он работает.


