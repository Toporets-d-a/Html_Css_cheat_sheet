# Instruction of CSS
## Св-ва элементов в css
```
box moddl: 
height (высота),
width (ширина), 
border(граница: 
(высота, цвет, внешний вид:
dotted-точками; 
solid-сплошной; 
dashed-тирешками.) 
```
### Padding (внутренний отступ)
```
padding:
порядок ввода:
левый, верхний, правый, 
нижний/ верх-низ, лево-право/ один 
для всех.
```
### Margin (внешний отступ)
```
Все св-ва работают как и в padding
```
### Св-ва размера объектов
```
max-width - максимальная ширина;
min-width - минимальная ширина;
max-height -максимальная высота;
min-height - минимальная высота;
для соотношения размеров 
используются проценты.
min и max главнее процентов.
```
### Float (св-во)
```
float - позволяет блочным элементам быть 
на одной строчке;возможные значения: left, right.
```
### Greed (св-во элементов в div)
```
greed - указывает св-ва по вертикали и по горизонтали.
```
### Margin (Св-во расположения элементов в div)
```
margin-left/right - отодвинуть на сколько возможно
(для justify-content, align-items, greed)
```
### Грамматика css
```
в css можно писать (class).(teg) .
в css можно писать (class).(teg), (teg2).
```
### Грамматика css
```
class="имя" для разделения типа на  классы
```
### Грамматика css
```
перед классом ставится точка в стилях если у разных 
тегов одинаковые св-ва их можно перечислять через запятую.
```
## Options of elements in conteiner
### Row (ряд)
```
row (default): left to right in (ltr); right to left in (rtl);
row-reverse: right to left in (ltr); left to right in (rtl).
```
Example:
```
.item {
  flex-basis: <length> | auto; /* default auto */
}
```
### Column (колонна)
```
column: same as row but top to bottom
column-reverse: same as row-reverse but bottom to top
```
Example:
```
.item {
  flex-basis: <length> | auto; /* default auto */
}
```
### Item (объект)
```
Отрицательные числа недействительны.
```
### Flex (Св-во элементов в div)
```
flex: (число) - какую часть места занимает объект. 
```
#### Flex-direction (Св-во div)
```
flex-direction: column/row(по умолчанию)- какая ось главная.
```
##### Values:
```
row, row-reverse, column, column-reverse;
```
##### Example:
```
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```
#### Flex-wrap (заворачивание)
```
nowrap (по умолчанию): все флекс-элементы будут в одной строке;
wrap: гибкие элементы будут переноситься на несколько строк сверху вниз;
wrap-reverse: элементы flex будут переноситься на несколько строк снизу вверх;
```
##### Values:
```
nowrap, wrap, wrap-reverse;
```
##### Example:
```
.container{
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```
#### Flex-grow (увеличение)
```
grow - если для всех элементов установлено значение 1, оставшееся место в
Контейнер будет распределен одинаково для всех
Отрицательные числа недействительны.
```
##### Values:
```
numbers (default 0);
```
##### Example:
```
.item {
  flex-grow: <number>;
}
```
#### Flex-shrink (сокращение)
```
Это определяет способность гибкого элемента сжиматься при необходимости.
Отрицательные числа недействительны.
```
##### Values:
```
numbers (default 1);
```
##### Example:
```
.item {
  flex-shrink: <number>;
}
```
#### Flex-flow (к главному)
```
flex-flow (Applies to: parent flex container element)
Это сокращенные свойства flex-direction и flex-wrap, 
которые вместе определяют основную и поперечную оси 
flex-контейнера. По умолчанию это строка nowrap.
```
##### Values:
```
flex-direction || flex-wrap;
```
##### Example:
```
.item {
flex-flow: <‘flex-direction’> || <‘flex-wrap’>
}
```
#### Flex-basis (основа)
```
Это определяет размер элемента по умолчанию перед распределением оставшегося пространства. 
Это может быть длинна или ключевое слово. 
Ключевое слово auto означает «посмотрите на мое свойство width или height» 
(которое временно выполнялось ключевым словом main-size до тех пор, пока оно не устарело). 
Ключевое слово content означает «изменить его размер в зависимости от содержимого элемента», 
это ключевое слово пока недостаточно хорошо поддерживается, поэтому сложно проверить и узнать, 
что делают его братья max-content, min-content и fit-content.
```
##### Values: 
```
length, auto (default auto);
example:

.item {
  flex-basis: <length>;
}
```
#### Justify-content
#### Values:
##### Flex-start 
```
(по умолчанию): элементы упакованы в начало строки
```
##### Flex-end 
```
предметы упакованы к концу строки
```
##### Center
```
пункты центрированы вдоль линии
```
##### Space-between 
```
предметы равномерно распределены по линии; первый элемент находится в 
начале строки, последний элемент в конце строки.
```
##### Space-around 
```
предметы равномерно распределены по линии с одинаковым пространством вокруг них. 
```
##### Space-evenly 
```
элементы распределяются таким образом, чтобы расстояние между 
любыми двумя элементами (и расстояние до краев) было одинаковым.
```
##### stretch (по умолчанию) 
```
растянуть, чтобы заполнить контейнер (все еще соблюдайте min-width / max-width)
```
#####flex-start
```
рай полей для перекрестного старта размещается на линии перекрестного старта
```
#####flex-end
```
углы элементов помещается на линию пересечения
```
##### Center 
```
пункты центрированы в поперечной оси
```
##### Baseline
```
элементы выровнены, такие как их базовые линии.
```
### Background color (цвет фона) и его св-ва.
example:
```
<p> {
background color: 157, 136, 93;
}
```
#### Backgrnd-image (использовать картинку как фон)
example:

<p> {
background color: 157, 136, 93;
}
```
#### Background-position (расположение картинки на фоне)
```  
Значения: top/centre/bottom,  left/centre/right.
example:
<div> {
background- position:top, right;
}
```
#### Background-repiat (заполнение фона нецелыми копиями картинки)
  
Значения: repeat-x/repet-y/no-repet.
example:
```
<div> {
background-repiat: no-repeat;
}
```
#### Background-size вместить всю картинку.

Значения: all, center, row, bottom, left, right.
example:
```
<div> {
background-size: all;
}
```
#### background: - можно перечислить все св-ва, кроме Size.
```
<div> {
backgrond: 
position:top, left;
repiat: no-repeat;
}
```
##### Примечание:
вначале пишут backgrond-color - на случай ошибки картинки.

##### Linear-gradient
Написать любые 2 цвета через запятую.
###### example:
```
.background-color {
linear-gradient: yellow, purple;
}
```
##### inherit (взять цвет из родительского блока).
example:
```
<div> {
background: inherit;
}
```
#### Filter (фильтр)
Св-ва:
blur (размытие);
greyscale (очёрнобелить);
example:
```
.Background of texts {
filter: blur="75%"
}
