

## 🧩 Блоки, элементы и модификаторы

### Блок `box`
Используется как контейнер для текста или заголовков.

### Элементы
- `box__title` — заголовок
- `box__text` — текст внутри заголовка или отдельного блока

### Модификаторы

#### Для текста:
- `box__text--clone` — включает `box-decoration-break: clone`
- `box__text--gradient-purple-pink` — градиент фиолетовый → розовый
- `box__text--gradient-green-blue` — градиент зелёный → синий
- `box__text--gradient-orange-red` — градиент оранжевый → красный

#### Для заголовков:
- `box__title--underline` — добавляет подчёркивание через `::before`
- `box__title--underline-purple-pink` — подчёркивание фиолетовый → розовый
- `box__title--underline-green-blue` — подчёркивание зелёный → синий
- `box__title--underline-orange-red` — подчёркивание оранжевый → красный

## 🖼 Примеры использования

### Текст с `box-decoration-break`
```html
<span class="box__text box__text--clone box__text--gradient-purple-pink">
  Привет, мир!
</span>
