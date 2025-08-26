# Box-decoration

Демонстрация различных декоративных эффектов для заголовков с использованием CSS и методологии БЭМ.

## О проекте

В проекте реализованы:

- Градиентный текст для заголовков
- Градиентное подчёркивание с помощью псевдоэлементов
- Пример заголовка с градиентным фоном через `::before` (см. инструкции ниже)

## Структура

- **index.html** — основная разметка с примерами заголовков
- **style.css** — стили для градиентов, подчёркиваний и оформления по БЭМ

## Использование

1. Склонируйте репозиторий или скачайте файлы.
2. Откройте `index.html` в браузере.
3. Изучите примеры декоративных заголовков.

## Как добавить заголовок с градиентным фоном

Добавьте в разметку:

```html
<div class="box">
  <h2 class="box__title box__title--bg-gradient">
    <span class="box__title-text">Заголовок с градиентным фоном</span>
  </h2>
</div>
```

И в `style.css`:

```css
.box__title--bg-gradient {
  position: relative;
  display: inline-block;
  overflow: hidden;
  padding: 0.3em 1.2em;
}

.box__title--bg-gradient::before {
  content: '';
  position: absolute;
  inset: 0;
  z-index: 0;
  border-radius: 0.5em;
  background: linear-gradient(90deg, #a259ff 0%, #ff6aab 100%);
  opacity: 0.8;
}

.box__title--bg-gradient .box__title-text {
  position: relative;
  z-index: 1;
  color: #fff;
  font-weight: 700;
}
```

## Применяемые технологии

- HTML5
- CSS3 (градиенты, псевдоэлементы)
- Методология БЭМ
