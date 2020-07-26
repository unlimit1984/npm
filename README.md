# Npm learning project

npm help
npm install -h
npm help-search update
npm help update
npm init
npm init --yes

npm [config] set init-author-name "unlimit1984”
npm set init-license "MIT”
npm init --yes
npm init -y //the same

npm config get init-author-name
npm get init-author-name
npm get init-license

npm config delete init-license

npm install moment //установка locally
npm i lodash //the same
npm i lodash -S //the same as --save
npm i lodash --save-dev
npm i lodash -D //the same as --save-dev
--global 
-g //the same as --global

npm --version
npm -V //the same

other shorthends:
https://docs.npmjs.com/misc/config#shorthands-and-other-cli-niceties


npm install moment --save //по идее добавляет зависимость в package.json, но у меня и без нее добавляет

npm install lodash --save-dev //сохраняет в раздел dev

npm uninstall moment --save //--save уже необязательно
npm uninstall lodash --save-dev //--save-dev необязательно

npm install moment -g //установит глобально
npm uninstall moment -g //удалит глобально

uninstall имеет синонимы/алиасы
un
remove
rm

npm list --depth 5
npm list -g
npm list --global true
npm list --global true --depth 1
npm list -g true --depth 1 //тоже самое
npm list --local true

"lodash": "^4.17.19"
4 - major version, инкрементится при разрушении существующей функциональности
17 - minor version, инкрементится при добавлении новой feature, но не рушит сущ. функционал
19 - patch version

npm install lodash@3.3.0
npm install lodash@4.14 //дай мне 4.14.X, но патч X возьми последний
npm install lodash@4 //дай мне 4.X.Y, но X и Y возьми последние

"lodash": "^4.14.1" //^ означает взять 4.X.Y, но возьми X и Y свежие
"lodash": "~4.16.1" //^ означает взять 4.16.Y, но возьми Y свежий
"lodash": "4.17.10" // возьми данную конкретную версию
"lodash": "*" // * означает взять последнюю версию библиотеки

"lodash": "^3.0.0"
npm update lodash //обновит версию до последней 3.X.Y (3.10.1)

npm update moment --dev --save-dev //обновит moment в devDependencies
--save-dev необязательно

npm update // обновит все dependencies, в том числе и devDependencies 
npm update -g // обновит все глобальные библиотеки
npm update -g gulp// обновит глобальную библиотеку gulp

npm install npm@latest -g // обновит саму npm глобально, проверь, что открыл консоль администратором

npm prune //удаляет все библиотеки с node_modules, которых нет в package.json (не забываем удалять package-lock.json

node app.js

npm run start
npm start //the same

npm run test
npm test //the same

