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
### Column (колонна)
```
column: same as row but top to bottom
column-reverse: same as row-reverse but bottom to top
```
### Item (объект)
```
Negative numbers are invalid.
```
### Flex (Св-во элементов в div)
```
flex: (число) - какую часть места занимает объект. 
```
#### Flex-direction (Св-во div)
```
flex-direction: column/row(по умолчанию)- какая ось главная.
```
#### Flex-wrap (заворачивание)
```
nowrap (default): all flex items will be on one line;
wrap: flex items will wrap onto multiple lines, from top to bottom;
wrap-reverse: flex items will wrap onto multiple lines from bottom to top;
```
#### Flex-grow (увеличение)
```
grow - If all items have it set to 1, the remaining space in the 
container will be distributed equally to all
Negative numbers are invalid.
```
#### Flex-shrink (сокращение)
```
This defines the ability for a flex item to shrink if necessary.
Negative numbers are invalid.
```
#### Flex-flow (к главному)
```
flex-flow (Applies to: parent flex container element)
Это сокращенные свойства flex-direction и flex-wrap, 
которые вместе определяют основную и поперечную оси 
flex-контейнера. По умолчанию это строка nowrap.
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
