# Пролог
	в основном освоим на лекции наследие html 4
эти технологии нужны чтобы декларировать то что видит пользователь на экране пользовательского агента

	язык разметки гипертекста
	гипертекст -- текст с гипер ссылками, типа как википедия
	но потом решили что да нужны картинки и т п

html -- структура документа. Пишите по минимому (идеально -- ноль) того, как должно выглядеть
	даже тег b (bold) считается теперь deprecated, вместо него лучше использовать strong -- показывает семантически что нужно увеличить здесь внимание, например проговорить громче для слепых
css -- как должно выглядеть
![[Pasted image 20240208210824.png|550]]
![[Pasted image 20240208210940.png|550]]
первая строчка (доктайп...) называется **прологом** -- типа говорит что дальше идет html...
# Html
дерево
*на самом деле корень это **document** , см слайд про **DOM***
- html
	- head -- метаинформация 
		- meta (**тег** без закрытия)
		- title
	- body
узлы дерева -- элементы и текстовые ноды
все после названия тега -- **атрибуты**, в формате ключ=значение

	html и xml похожи но не наследуются между собой, у них просто **кажется** есть общий предок
	
	заглушка текста Lorem Ipsum
директива **link**  -- говорит подключи данный .css файл к отображению 
![[Pasted image 20240208215047.png|400]]

## Элементы (теги?)
Элементы(теги?) можно разделить на:
- **inline**-элементы -- типа кусочек строки, могут даже начаться на одной строке и перенестись на другую строку. 
	Примеры: p, div, main, header, section, article
- **блоковые** (блочные) -- по умолчанию занимает в **ширину** сколько может, а **высоту** сколько минимально нужно. 
Эти режимы отображения можно насильственно менять (см [[2 -- HTML + CSS#^displaySlide]])
по сути в html теги одного типа делают одно и тоже, разные названия передают семантику
ну только **div и span не обладают семантикой**, это простой блоковый и inline элементы соответственно

Всякие теги:
- p -- paragraph
	параграф текста
	блочный
- a - anchor (якорь) 
	ссылка
	есть обязательный тег **href**
	inline
- span 
	inline-элемент
- nav -- навигация
	типа менюшка
	логично внутри юзать ul { li li li}
- footer 
	хуйня внизу, написать копирайт

## Блоковые элементы (слайд)
![[Pasted image 20240208223235.png|550]]
margin -- внешний отступ
border -- граница
padding -- отступ контента от бордера

когда мы руками устанавливаем width/height, то по дефолту он устанавливается для контента
чтобы это поведение менять юзаем box-sizing
![[Pasted image 20240208224404.png]]
значения margin-box кажется не существует

упражнение: объяснить почему будет по разному себя вести ширина блоков при добавлении width100% :
![[Pasted image 20240208224255.png|201]]

### display: (слайд)
^displaySlide

![[Pasted image 20240208224558.png|425]] 

к inline неприменимы верхние/нижние отступы и ширина
inline-block -- не разрывает строку, но можно указывать левые/правые отступы и т п

### Позиционирование = position: (слайд)
![[Pasted image 20240208224916.png|475]]
речь идет про блоковые элементы
**relative** -- нарисовали как статик, а потом вырезали и подвинули (все размеры не меняются)
**absolute** -- забываем про контекст, отображаем от какой-то "точки отсчета", другие элементы про него не знают (не должны знать, забывают)
**точка отсчета**: дефолтно -- левый верхний угол, иначе -- идем вверх по дереву до первого элемента с **position: relative**
**fixed** -- абсолютно относительно левого верхнего угла браузера а не документа, например для уведомлений

### Поплавки
![[Pasted image 20240208225821.png|475]]
**ИНФОРМАЦИЯ НА СЛАЙДЕ ОЧЕНЬ ВАЖНАЯ ПРОЧИТАТЬ ВНИКНУТЬ И ПРОЧИТАТЬ ЕЩЕ РАЗ!!!!**


## Атрибуты элементов
все свои (не стандартные) атрибуты нужно начинать с "data-"
- **атрибут class**
	говорит к какому классу принадлежит элемент
	один элемент может принадлежать нескольким классам
	![[Pasted image 20240208213819.png|300]] 
	-- классы перечисляются через пробел
- **атрибут title**
	какой текст выводится при наведении курсора
- **атрибут alt**
	какой текст вывести вместо картинке если она не смогла подгрузиться

## REM
"root-em"
размер шрифта в документе
величина размера


## header появился в html5 ? #проверить 
проверить

# CSS
![[Pasted image 20240208215331.png|525]]
состоит в основном из правил
как выглядит правило:
```
селектор : {
	ключ1: значение1;
	ключ2: значение2;
	...
}
```
## Селектор, DOM
Селектор -- декларативный запрос к **DOM** (*Document Object Model* = дереву документа) "найди набор элементов из этого дерева"
![[Pasted image 20240208214240.png|525]]
### Составные селекторы
	"более сложные способы запрашивать узлы из DOM-а"
контролировать связки скобками **нельзя**))

- пробел =  "предок->потомок"
	note: потомок, а не сын
![[Pasted image 20240208221831.png|162]]
- больше = "родитель->ребенок"
![[Pasted image 20240208221926.png|129]]
- запятая=объединение путей, "или"
![[Pasted image 20240208222127.png|250]]
- двоеточие=псевдоклассы -- всякие штуки)) 
![[Pasted image 20240208222919.png|475]]
![[Pasted image 20240208223026.png|155]] ![[Pasted image 20240208223054.png|147]]
![[Pasted image 20240208234907.png|250]]
**Не путать!**
 "пэшка" с id="mike":
![[Pasted image 20240208222239.png]]
 id="mike" у которого есть предок "пэшка":
![[Pasted image 20240208222408.png]]
### Примеры

```
p : { -- все теги <p>
}

* : { -- ВСЕ элементы
}

#[идентефикатор] { 
} -- для 
<[тег] id="[идентефикатор]">...</>

предполагается что id уникальны

.[класс] { 
} -- для всех 
<[тег] class="[класс1 класс ...]">...</>



```

![[Pasted image 20240208220048.png|255]]
![[Pasted image 20240208220129.png|138]] ![[Pasted image 20240208220152.png|173]]
вроде можно и без кавычек
## Еще фишки
![[Pasted image 20240208235207.png|130]]
min_width 800px -- ширина не меньше 800 пикселей (если окно меньше то будет прокрутка а не еще большее сжатие)
![[Pasted image 20240209000457.png|325]]
псевдо-элементы before after


# normalize.css
у браузера есть встроенные типа-css-ки которые говорят какие отступы делать на элементах по умолчанию
хотим ? верстку которая будет одинаково смотреться во всех бразерах в мире
есть два пути:
1. ресетнуть нахуй все
2. сделать нормалайз -- сбросить стили до нормального одинакового четкого значения во всех браузерах
#непонел 



# коллизии
css -- при коллизиях правил движки обычно стараются применить правило более специфичного селектора (например по id специфичнее чем по tag-name)
но **вроде** четких правил нет

можно повышать значимость правила))
![[Pasted image 20240208220654.png]]