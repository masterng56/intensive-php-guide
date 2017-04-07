Учебник по PHP
============

- собранная версия учебника лежит на [gh-pages](http://html-academy.ru/intensive-php-guide/);
- публикация происходит автоматически из `master`-ветки;
- собирается с помощью [Jekyll](https://jekyllrb.com/);
- все разделы учебника лежат в папке `guide`.

### Как запустить учебник локально

1) Убедитесь, что у вас стоят `Ruby`, `RubyGems` и выполнены все [остальные условия](https://jekyllrb.com/docs/installation/).

2) Установите Jekyll и Bundler с помощью RubyGems
```bash
$ gem install jekyll bundler
```

3) Если у вас официальная инструкция не работает из-за отсутствия доступа к Ruby, находящимся в системном разделе, то можно воспользоваться вот такой:

  - убедитесь, что установлен `xcode`
  ```bash
  $ sudo xcode-select --install
  ```

  - установите `rbenv` с помощью [Homebrew](https://brew.sh/index_ru.html)
  ```bash
  $ brew install rbenv
  ```

  - в зависимости от того, какой консолью пользуетесь, добавьте в конец файла `~/.zshrc` или `~/.bash_profile` строку
  ```
  "$(rbenv init -)"
  ```

    > узнать, какая консоль используется у вас, можно с помощью команды `$ echo $SHELL`

    > для показа всех, даже скрытых и системных, файлов можно воспользоваться командой `ls -a`

  - установите Ruby с указанием нужной/стабильной версии, например
  ```bash
  rbenv install 2.3.0
  ```

  - с помощью `rbenv` выберите установленную версию Ruby
  ```bash
  rbenv global 2.3.0
  ```

  - в новом окне терминала проверьте, что команда
  ```bash
  gem env home
  ```
  возвращает путь к пользовательской папке, а не системной

  - установите Jekyll и Bundler с помощью RubyGems
  ```bash
  $ gem install jekyll bundler
  ```

4) Запустите сборку и сервер из папки проекта

```bash
$ bundle exec jekyll serve
```

---

## Как предложить изменения

* Сделайте форк репозитория
* Внесите изменения (можно вносить много и долго)
* Когда будете готовы, создайте из вашего форка пулреквест и опишите, что вы сделали
* Дождитесь обсуждения ваших изменений и приёма их в мастер
