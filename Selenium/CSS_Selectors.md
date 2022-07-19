[Selectors](#T1) <br>
[Pseudo classes](#T2) <br>
[Attribute selectors](#T3) <br>
[Picture](#T4) 

<a name="T1"></a>  
## Selectors
  
| Selector | Atribut |
|----------|---------|
|*         |all elements|
|div       |all div tags|
div,p      |all divs and paragraphs
div p      |paragraphs inside divs
div > p    |all p tags, one level deep in div
div + p    |p tags immediately after div
div ~ p    |p tags preceded by div
.classname |all elements with class
#idname    |element with ID
div.classname|divs with certain classname
div#idname |div with certain ID
#idname *  |all elements inside #idname

<a name="T2"></a> 
## Pseudo classes
![1](https://user-images.githubusercontent.com/84935915/179760336-6bfe5f4f-0958-4808-8b0a-13a9489cb031.png)

| Selector            | Atribut
----------------------|---------------------
|a:link               |link in normal state|
a:active|link in clicked state
a:hover|link with mouse over it
a:visited|visited link
p::after{content:"yo";}|add content after p
p::before|add content before p
input:checked|checked inputs
input:disabled|disabled inputs
input:enabled|enabled inputs
input:focus|input has focus
input:in-range|value in range
input:out-of-range|input value out of range
input:valid |input with valid value
input:invalid |input with invalid value
input:optional   |no required attribute
input:required|  input with requred attribute
input:read-only |with readonly attribute
input:read-write |no readonly attrib.
div:empty |element with no children
p::first-letter |first letter in p
p::first-line |first line in p
p:first-of-type |first of some type
p:last-of-type |last of some type
p:lang(en) |p with en language attribute
:not(span) |element that's not a span
p:first-child |first child of its parent
p:last-child |last child of its parent
p:nth-child(2) |second child of its parent
p:nth-child(3n+1) |nth-child (an + b) formula
p:nth-last-child(2) |second child from behind
p:nth-of-type(2) |second p of its parent
p:nth-last-of-type(2) |...from behind
p:only-of-type |unique of its parent
p:only-child |only child of its parent
:root |documents root element
::selection|portion selected by user
:target|highlight active anchor

[Selectors](#T1) <br>
[Pseudo classes](#T2) <br>
[Attribute selectors](#T3) <br>
[Picture](#T4)

<a name="T3"></a> 
## Attribute selectors

| Selector            | Atribut
----------------------|---------------------
`a[target]` | links with a target attribute
`a[target="_blank"]`        |      links which open in new tab
`[title~="chair"]`|title element containing a word
`[class^="chair"]`|class starts with chair
`[class(palka)="chair"]`|class starts with the chair word
`[class*="chair"]`|class contains chair|
`[class$="chair"]`|class ends with chair|
`input[type="button"]`|specified input type|

<a name="T4"></a> 
## Picture
![CSS - омбинированные селекторы](https://user-images.githubusercontent.com/84935915/179619144-0a66557c-f4a2-492f-a859-4ead65209053.png)

## Поиск по тексту

Пример:

![1](https://user-images.githubusercontent.com/84935915/179760403-099fe55c-29ac-409a-a504-59df79b9a659.png)

Как видим id явно сгенерирован и привязаться к нему нельзя, класс тоже не внушает доверия, кроме того Selenium не разрешает использовать сложносоставные имена в локаторе className, но тут есть текст, который решает проблему: `//a[text()=’Contact us’]`

[Selectors](#T1) <br>
[Pseudo classes](#T2) <br>
[Attribute selectors](#T3) <br>
[Picture](#T4) 
