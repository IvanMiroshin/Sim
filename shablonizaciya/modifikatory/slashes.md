# slashes

Экранирует строку с помощью слешей. Возвращает строку с обратным слешом перед символами, которые нужно экранировать. Экранируются одиночная кавычка \('\), двойная кавычка \("\), обратный слеш \(\\).

### **Синтаксис**

```text
string $var:slashes;
```

\*\*\*\*

### **Пример использования**

Входные данные:

```php
Array
(
    ['myvar'] => "\It's a \string"
)
```

Шаблон:

```markup
<p data-sim="content($data.myvar:slashes);"> … </p>
```

Результат выполнения:

```markup
<p>\\It\'s a \\string</p>
```
