# Справочник по выравниванию контента в HTML документах с помощью CSS и параметров display: flex

## Введение

Flexbox (Flexible Box) — это модуль CSS, который позволяет легко создавать гибкие и адаптивные макеты. Он предоставляет множество возможностей для выравнивания и распределения элементов внутри контейнера. В этом справочнике мы рассмотрим основные свойства и параметры, которые помогут вам выравнивать контент с помощью Flexbox.

## Основные свойства Flexbox

### display: flex

Чтобы начать использовать Flexbox, нужно установить контейнеру свойство `display: flex`. Это превращает контейнер в flex-контейнер и позволяет использовать все остальные свойства Flexbox.

```css
.container {
  display: flex;
}
```

### flex-direction

Свойство `flex-direction` определяет направление главной оси (main axis) flex-контейнера.

- `row` (по умолчанию): слева направо.
- `row-reverse`: справа налево.
- `column`: сверху вниз.
- `column-reverse`: снизу вверх.

```css
.container {
  display: flex;
  flex-direction: row; /* или column, row-reverse, column-reverse */
}
```

### justify-content

Свойство `justify-content` выравнивает элементы по главной оси.

- `flex-start` (по умолчанию): элементы выравниваются в начале контейнера.
- `flex-end`: элементы выравниваются в конце контейнера.
- `center`: элементы выравниваются по центру контейнера.
- `space-between`: элементы равномерно распределяются с промежутками между ними.
- `space-around`: элементы равномерно распределяются с равными промежутками вокруг них.
- `space-evenly`: элементы равномерно распределяются с равными промежутками между ними и по краям контейнера.

```css
.container {
  display: flex;
  justify-content: center; /* или flex-start, flex-end, space-between, space-around, space-evenly */
}
```

### align-items

Свойство `align-items` выравнивает элементы по поперечной оси (cross axis).

- `stretch` (по умолчанию): элементы растягиваются, чтобы заполнить контейнер.
- `flex-start`: элементы выравниваются в начале контейнера.
- `flex-end`: элементы выравниваются в конце контейнера.
- `center`: элементы выравниваются по центру контейнера.
- `baseline`: элементы выравниваются по базовой линии.

```css
.container {
  display: flex;
  align-items: center; /* или stretch, flex-start, flex-end, baseline */
}
```

### align-content

Свойство `align-content` выравнивает строки flex-контейнера по поперечной оси, если высота контейнера больше суммарной высоты строк.

- `stretch` (по умолчанию): строки растягиваются, чтобы заполнить контейнер.
- `flex-start`: строки выравниваются в начале контейнера.
- `flex-end`: строки выравниваются в конце контейнера.
- `center`: строки выравниваются по центру контейнера.
- `space-between`: строки равномерно распределяются с промежутками между ними.
- `space-around`: строки равномерно распределяются с равными промежутками вокруг них.
- `space-evenly`: строки равномерно распределяются с равными промежутками между ними и по краям контейнера.

```css
.container {
  display: flex;
  flex-wrap: wrap; /* необходимо для использования align-content */
  align-content: center; /* или stretch, flex-start, flex-end, space-between, space-around, space-evenly */
}
```

### flex-wrap

Свойство `flex-wrap` определяет, будут ли элементы переноситься на новую строку, если они не помещаются в одну строку.

- `nowrap` (по умолчанию): элементы не переносятся на новую строку.
- `wrap`: элементы переносятся на новую строку.
- `wrap-reverse`: элементы переносятся на новую строку в обратном порядке.

```css
.container {
  display: flex;
  flex-wrap: wrap; /* или nowrap, wrap-reverse */
}
```

### flex-grow, flex-shrink, flex-basis

Эти свойства применяются к flex-элементам и определяют, как они будут растягиваться, сжиматься и занимать место в контейнере.

- `flex-grow`: определяет, как элемент будет растягиваться относительно других элементов.
- `flex-shrink`: определяет, как элемент будет сжиматься относительно других элементов.
- `flex-basis`: определяет начальный размер элемента.

```css
.item {
  flex-grow: 1; /* или любое другое значение */
  flex-shrink: 1; /* или любое другое значение */
  flex-basis: auto; /* или любое другое значение */
}
```

### order

Свойство `order` определяет порядок отображения flex-элементов. Элементы с меньшим значением `order` отображаются раньше.

```css
.item {
  order: 1; /* или любое другое значение */
}
```

## Примеры использования

### Пример 1: Центрирование элементов

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
</div>
```

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.item {
  padding: 20px;
  background-color: lightblue;
  margin: 10px;
}
```

### Пример 2: Равномерное распределение элементов

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
</div>
```

```css
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 100vh;
}

.item {
  padding: 20px;
  background-color: lightblue;
  margin: 10px;
}
```

### Пример 3: Многострочный flex-контейнер

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
  <div class="item">Item 4</div>
  <div class="item">Item 5</div>
</div>
```

```css
.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  align-content: space-around;
  height: 100vh;
}

.item {
  padding: 20px;
  background-color: lightblue;
  margin: 10px;
  flex-basis: 200px;
}
```
