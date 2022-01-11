# Аккордеон на чистом JavaScript

Плагин позволяет оживить аккордеоны на сайте

## Подключение

1. Подключить стили и скрипты

```html
<!-- Styles -->
<link rel="stylesheet" href="plugin/CgAccordion.css" />

<!-- JavaScript -->
<script src="plugin/CgAccordion.js"></script>
```

2. Создание разметки HTML

```html
<div class="accordion" data-accordion="one">
  <div class="accordion__top">
    <span class="accordion__top-title"><!-- Title --></span>
    <svg class="accordion__top-icon" width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M3.87002 6.16498L2.10003 7.93498L12 17.835L21.9 7.93498L20.13 6.16498L12 14.295L3.87002 6.16498V6.16498Z"/>
    </svg>
  </div>
  <div class="accordion__body">
    <!-- Body -->
  </div>
</div>
```

3. Инициализировать JS

```javascript
const accordion = new CgAccordion('.accordion', {
  // options
});
```

## Параметры

`activeClass` - класс который будет добавляться к активному элементу (по умолчанию: 'accordion--active')

`bodyClass` - класс для основного контента аккордеона
(по умолчанию: 'accordion\_\_body')

`dataAttribute` - data-атрибут позволяющий объединять аккордеоны в группы (по умолчанию: 'accordion')

`topClass` - класс для верхней части аккордеона (по умолчанию: 'accordion\_\_top')

`speed` - скорость анимации
