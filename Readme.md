
# Категории продуктов электронной коммерции

## Цель

Основная цель - каталогизировать и стандартизировать категории и опции продуктов электронной коммерции.

Вы можете внести свой вклад, для этого не нужно регистрироваться на каком-то сайте, ни у кого просить доступ, вы просто присылаете коммит в этот репозиторий.

## Формат

Все файлы проекта ведутся в формате [YAML][1], имена допускают символы `/[^a-zA-Z-а-яА-Я-0-9_,-~]/`
В любой момент вы можете склонировать этот репозиторий и развернуть у себя на сервере. Также вы можете читать файлы прямо на GitHub.

## Структура опции

* `caption` - аголовок
* `unit` - единица измерения
* `description` - краткое описание
* `type` - тип
* `required` - флаг указывающий что опция является обязательной
* `collection` - флаг указывающий что опция является набором значений
* `option` - массив предустановленных значений опции

Пример описания опции *Сезон*

```
caption: Сезон
unit: ''
description: 'Укажите сезонность товара'
key: season
type: option
required: false
collection: false
option:
    - Весна
    - Демисезон
    - Еврозима
    - Зима
    - Лето
    - 'На любой сезон'
    - Осень
```

## Виды опций

* `text` - текстовая
* `int` - числовая целое значение
* `float` - числовая дробное значение
* `bool` - булевая
* `option` - опциональная

[1]: https://yaml.org/spec/1.2/spec.html
