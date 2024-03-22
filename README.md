# webpackStart

#Start
Данное руководство будет описывать создание проекта с 0. Оно будет разбито на шаги и в этом описании, каждый шаг будет помечен заголовком №{Название шага} и закреплен коммитом с аналогичным названием
Проект будет представлять из себя SPA на React
Для комфортной разработки будут введены TypeScript, Eslint, Prettier, pre-commit линтеры
Для сборки проекта будет использоваться webpack

#Шаг-1

- для начала работы уcтановим package.json в проект (npm init -y)
- Создадим папку src в коре проекта. Эта папка будет содержать всю логику нашего приложения.
- Создадим папку configs в корне приложения, эта папка будет содержать все конфигурации, которые касаются настрйоки webpack
- Внутри папки src создадим index.js. Этот файл будет являться точкой входа в нашей приложение.
- Далее установим пакеты для взаимодействием с вебпаком npm i -D webpack webpack-cli. Флаг -D усианавливает зависимости как devDepencies

Вопросы этого шага:

- Для чего нужен package.json?
- Для чего нужен package-lock.json?
- Чем отличаются минорные, мажорные, патч версии?
- Чем отличаются dependies и devDependies, какие пакеты класть можно в эти поля?
- Перед пакетами также могут стоять такие символы, как ^ ~ < > <= >= что они обозначают?
- Как удалить зависимости из package.json?
- Для чего нужна папка node_modules? Стоит ли эту папку отслеживать гиту?
- Отслеживает ли гит пустые папки? Как заставить гит отслеживать пустые папки и когда это нужно?
- В чем разница между npm install(npm i) и npm ci? В каких случаях разумно использовать эти команды?
- Как работает SPA (single-page-apllication)?
- Для чего используют webpack? Какие вещи он упрощает?
- Для чего нужен .gitignore файл?

Доп.вопросы для прокачки

- Зачем нужен ssh ключ для гита?
- Как установить ssh ключ у себя на ПК и передать это гитхабу(гитлабу и прочим)?
- git reset HEAD, git push --force, git stash, git commit --ammend, git commit cherry-pick
- что такое npm?

- https://softovik.net/zachem-nuzhen-package-lock-json-i-package-json
- https://ru.hexlet.io/qna/javascript/questions/kak-rabotaet-package-json#:~:text=%D0%A4%D0%B0%D0%B9%D0%BB%20package.,%D0%B7%D0%B0%20%D0%BF%D0%BE%D1%8F%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5%D0%BC%20%D0%BD%D0%BE%D0%B2%D1%8B%D1%85%20%D0%B2%D0%B5%D1%80%D1%81%D0%B8%D0%B9%20%D0%BF%D0%B0%D0%BA%D0%B5%D1%82%D0%BE%D0%B2.
- https://habr.com/ru/companies/domclick/articles/510812/
- https://builtin.com/software-engineering-perspectives/npm-ci-vs-npm-install
- https://dev.to/grawl/pochiemu-nie-nado-kommitit-papku-nodemodules-e37

#Шаг-2
- Для начала внедрим TS на проект (npm i typescript -D)
- В корне проекта создадим файл tsconfig.json, подробнее обо всех опциях этого файла можно узнать тут https://habr.com/ru/articles/542234/ или в офиц доке TS
- Далее внедряем eslint, делаем npx eslint init
- Устанавливаем prettier по гайду https://dev.to/eprikhodko/eslint-prettier-vs-code-create-react-app-airbnb-52bc#eslint-%D0%B2-create-react-app

Самостоятельно:
- Завязываем VS Code на претир и эслинт вашего проекта
- Установить stylelint для css файлов (scss, module.scss)
- Установить линтеры для прекомита и комита (ищем commitlint, husky, lint-staged)

После всех этих манипуляций у вас будут помощники, которые будут следить за оформлением кода, не дадут коду, который имеет ошибки попасть в удаленный репозиторий. Также эти поомщники не позволят допустить глупые ошибки в коде, среда будет их подсвечивать

- Что такое TypeScript? Зачем он нужен? Для чего tsconfig файл?
- Что такое eslint? Зачем он нужен? Для чего eslintrc файл?
- Что такое eslint? Зачем он нужен? Для чего eslintrc файл?
- Что такое prettier? Зачем он нужен? Для чего prettierrc файл?
- Что такое stylelint? Зачем он нужен? Для чего stylelint файл?
- Зачем нужно настраивать проверку файлов при коммите?

