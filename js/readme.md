## Домашнее задание по JS
Реализация пользовательских жестов в рамках игры «Dungeon of Doom».

Прохождение игры состоит из последовательного открытия дверей и в конце открытия сундука. Каждая дверь представляет из себя мини-загадку для решения которой игрок должен сделать какой-либо жест. Жесты могут быть как для одного указателя, так и для нескольких.

Для открытия первой двери игрок должен одновременно зажать три кнопки, чтобы дверь открылась. Это невозможно сделать на компьютере, поэтому пройти эту дверь можно только с мобильного устройства с multi-touch (т.е. с помощью любого смартфона).

Остальные две двери и сундук предлагается реализовать вам. Графическое оформление также можно менять по желанию.

#### Файлы
- [sample](sample) — папка с самой игрой
- [sample/index.html](sample/index.html)
- [sample/css](sample/css) — папка со стилями. В файле [sample/css/app.css](app.css) основные стили.
- [sample/js/doorBase.js](sample/js/doorBase.js) — базовый класс двери. От него наследуются все двери и сундук.
- [sample/js/doorOthers.js](sample/js/doorOthers.js) — реализации дверей в игре. Первая дверь реализована полноценно и может быть использована в качестве примера. Остальные двери реализованы по принципу "любой клик на двери её откроет". Вам предлагается заменить эту логику на более сложную.

Свой код дверей предполагается писать в рамках
```js
// ==== Напишите свой код для открытия сундука здесь ====
...
// ==== END Напишите свой код для открытия сундука здесь ====
```
а также в `index.html` в DOM-элементах `.popup_level_1`, `popup_level_2` и `popup_level_3`.


#### Основные техники, которые должны быть реализованы:
- Использование Pointer Events.
- Жест открытия для одной двери.

#### Также приветствуется реализация дополнительных техник на более высокую оценку:
- Сложные жесты, которые будет непросто сделать игроку. Желательно с использованием нескольких указателей (пальцев).  Можно вдохновляться играми серии The Room, всевозможными пазлами и загадками в квестах. Например:
  - Для открытия двери необходимо сдвинуть в разные стороны несколько затворов.
  - За определенное время покрутить по кругу несколько рычагов.
  - "Восстановить" механизм открытия двери перемещением шестеренок в соответствующие им пазы.
- Сделать разные жесты открытия для всех дверей и сундука.

#### Вспомогательные материалы
Графические материалы можно взять с http://kenney.nl/assets/ или любого другого сайта с бесплатными ресурсами для игр. В этой игре используются изображения из набора http://kenney.nl/assets/platformer-pack-redux.

## Куда и когда присылать
- Работы присылать на dndushkin@yandex-team.ru
  - Желательно сопроводить работу кратким описанием основных фишек (чтобы при оценке ничего не забылось)
  - Лучше ссылками на сверстанную страницу (например, разместить на бесплатном [GitHub Pages](https://pages.github.com/) с помощью gh-pages)
  - На крайний случай просто архивом
- Тема: "ДЗ по JS (фамилия и имя)"
- Срок — до 14 июля 12:00
