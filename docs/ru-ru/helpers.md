# Doc helper

docsify расширяет синтаксис Markdown, чтобы сделать ваши документы более читаемыми.

## Важный контент

Важный контент как:

```markdown
!> **Время** деньги, мой друг!
```

отобразится как:

!> **Время** деньги, мой друг!

## Основной совет

Совет как:

```markdown
?> _TODO_ unit test
```

отобразится как:

?> _TODO_ unit test

## Игнорировать компиляцию ссылки

В некоторый момент времени вам понадобится добавить какой-то другой относительный путь к ссылке, вам нужно будет сообщить, что вам не нужно компилировать эту ссылку. Например

```md
[link](/demo/)
```

Он будет скомпилирован в `<a href="/#/demo/">link</a>` и будет загружен `/demo/README.md`. Может быть, вы хотите перейти на `/demo/index.html`.

Теперь вы можете сделать это

```md
[link](/demo/ ':ignore')
```

Вы получите html `<a href="/demo/">link</a>`. Не волнуйтесь, вы все равно сможете установить заголовок для ссылки.

```md
[link](/demo/ ':ignore title')

<a href="/demo/" title="title">link</a>
```

## Установить целевой атрибут для ссылки

```md
[link](/demo ':target=_blank')
[link](/demo2 ':target=_self')
```

## Отключить ссылку

```md
[link](/demo ':disabled')
```

## Github список задач

```md
* [ ] foo
* bar
* [x] baz
* [] bam <~ not working
  * [ ] bim
  * [ ] lim
```

* [ ] foo
* bar
* [x] baz
* [] bam <~ not working
  * [ ] bim
  * [ ] lim

