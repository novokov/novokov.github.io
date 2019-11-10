---
title: Настройка Sublime Text 3
date: 2018-09-22 
categories:
  - uncategorized
tags:
  - in process
---


Для начала отключим проверку обновлений 
Для этого сделем следующее:
Preferences -> Settings - User и добавить туда следующую строчку:

```
"update_check": false, 
```

## 1. Настройка Package Control
- Нажимаем ctrl+shift+p
- вводим туда install package control
- появится окошко , что все ок 

## 2. Установка пакетов

- Нажимаем ctrl+shift+p
- открываем package control
- устанавливаем пакеты:
- emmet
- AutoFileName - дополняет код при написании путей до файлов в вёрстке;
- Gist - подключает в Sublime Text возможность использовать сервис сниппетов кода GitHub Gist. Урок по Gist;
- Sass - плагин для подсветки Sass синтаксиса в Sass и Scss файлах. Раскрывает Emmet в Sass файлах.
- One Dark Color Scheme - цветовая схема для подсветки кода;
- One Dark Material - Theme - тема оформления UI Sublime Text.
- Sublime Jekyll - чтобы как нормальный человек работать с jekyll сайтов в саблайме.

## 3. Открываем preferences - Settings и вставляем пресет

```
{
    "show_definitions": false,
    "auto_complete": false,
    "bold_folder_labels": true,
    "color_scheme": "Packages/One Dark Material - Theme/schemes/OneDark.tmTheme",
    "fold_buttons": false,
    "font_size": 10,
    "highlight_line": true,
    "indent_guide_options":
    [
        "draw_normal",
        "draw_active"
    ],
    "line_padding_bottom": 2,
    "line_padding_top": 2,
    "margin": 2,
    "material_theme_compact_sidebar": true,
    "material_theme_compact_panel": true,
    "material_theme_small_statusbar": true,
    "material_theme_small_tab": true,
    "tab_size": 2,
    "theme": "OneDarkMaterial.sublime-theme",
    "word_wrap": "false",

}
```

## 4. Неплохо бы поставить пакет sublime-jekyll
<a href="https://sublime-jekyll.readthedocs.io/en/latest/" target="_blank">Документация пакета sublime-jekyll</a>

1. Устанавлиаем пакет через `ctrl + shift + p` введя jekyll.
2. Установили, ок.
3. Далее в User-Settings дописываем конфигурацию для пакета.
Локальный реп лежит всегда по пути `D:\\Documents\\Github Repository\\sitename.github.io`
Дописываем (копипастим) следующие строчки в user settings

```
"Jekyll":
    {
        "jekyll_drafts_path": "D:\\Documents\\Github Repository\\akulich1.github.io\\_drafts",
        "jekyll_posts_path": "D:\\Documents\\Github Repository\\akulich1.github.io\\_posts",
        "jekyll_uploads_path": "D:\\Documents\\Github Repository\\akulich1.github.io\\_uploads",
        "jekyll_templates_path": "D:\\Documents\\Github Repository\\akulich1.github.io\\_templates",
    },
```

4. Все, все команды для плагина доступны из `ctrl + shift + p`. Описание к командам <a href="https://sublime-jekyll.readthedocs.io/en/latest/commands.html" target="_blank">тут</a>

Код шаблона `template-name.yaml`, что в `_templates` лежит.

```yaml
# defaul post
---
title: basic
categories:
  - uncategorised yet
tags:
  - untagged yet
---

<!-- image
![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url) 

-->

<!-- Link
[GitHub](http://github.com)
--->

<!-- to-do list
- [x] this is a complete item
- [ ] this is an incomplete item
-->

<!-- Table

First Header | Second Header
------------ | -------------
Content cell 1 | Content cell 2
Content column 1 | Content column 2

-->
```

## 5. Ну и последним шагом поставим md preview в sublime

<a href="https://packagecontrol.io/packages/MarkdownLivePreview">Ссылка на пакет</a>

- через `ctrl + shift + p` устанавливаем markdown livepreview
- Из md файла превью запускается через `alt+ m`