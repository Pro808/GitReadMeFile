# Readme file formatting

Примеры форматирования файла `readme.md` <br />

Описание стандарта можно найти по этой ссылке [Документация](https://github.github.com/gfm/ "Документация")

Похожий проект на гитхабе [GnuriaN](https://github.com/GnuriaN/format-README/blob/master/README.md "GnuriaN")

# Разделительная черта
___
***
---
`___, ***, ---`

> Использование `-` форматирует верхний текст, как заголовок 1-го уровня.

# Заголовки

Заголоввки задаются сиволом `#`, уровень корректируется количеством шарпов; <br/>

# Заголовок 1-го уровня `#{text}`

## Заголовок 2-го уровня `##{text}`

### Заголовок 3-го уровня `###{text}`

#### Заголовок 4-го уровня `####{text}`

##### Заголовок 5-го уровня `#####{text}`

###### Заголовок 6-го уровня `######{text}`

# Математические выражения

Математические выражения в `*.md` github не поддерживает. Есть возможность 
создать документацию на странице Wiki проекта, используя `*.rst (ReStructuredText)`.

Подробнее можно узнать по ссылке [ReStructuredText](https://github.com/DevDungeon/reStructuredText-Documentation-Reference#sphinx "ReStructuredText")

Чтобы включить поддержку в `*.md` можно воспользоваться двумя ресурсами:

- [latexEqnEditor](https://www.codecogs.com/latex/eqneditor.php)
  
  Формат, получаемо выражения, `svg`. В футере страницы выбираем `url`, комируем содержимое:
  ```text
  https://latex.codecogs.com/svg.latex?\fn_jvn&space;\large&space;\bigcap&space;\bigcup&space;{a_{b}}^{c}
  Оборачиваем, как ссылку ![](https://latex.codecogs.com/svg.latex?\fn_jvn&space;\large&space;\bigcap&space;\bigcup&space;{a_{b}}^{c})
  ```
  
  ![](https://latex.codecogs.com/svg.latex?\fn_jvn&space;\large&space;\bigcap&space;\bigcup&space;{a_{b}}^{c})
  
- [tex-image-link-generator](https://tex-image-link-generator.herokuapp.com/)

  Вводим выражение и копируем содержимое `Markdown`
  
  ```text
  ![\begin{align*}
  R(g) &= \frac{1}{n} \sum_{i=1}^{n} \ell(y_i,g(x_i))\\
  &=\frac{1}{2n} (\mathbf{X}\boldsymbol{w}-\mathbf{y})^T (\mathbf{X}\boldsymbol{w}-\mathbf{y})
  \end{align*}
  ](https://render.githubusercontent.com/render/math?math=%5CHuge+%5Ctextstyle+%5Cbegin%7Balign%2A%7D%0AR%28g%29+%26%3D+%5Cfrac%7B1%7D%7Bn%7D+%5Csum_%7Bi%3D1%7D%5E%7Bn%7D+%5Cell%28y_i%2Cg%28x_i%29%29%5C%5C%0A%26%3D%5Cfrac%7B1%7D%7B2n%7D+%28%5Cmathbf%7BX%7D%5Cboldsymbol%7Bw%7D-%5Cmathbf%7By%7D%29%5ET+%28%5Cmathbf%7BX%7D%5Cboldsymbol%7Bw%7D-%5Cmathbf%7By%7D%29%0A%5Cend%7Balign%2A%7D%0A)
  ```
  
  ![\begin{align*}
  R(g) &= \frac{1}{n} \sum_{i=1}^{n} \ell(y_i,g(x_i))\\
  &=\frac{1}{2n} (\mathbf{X}\boldsymbol{w}-\mathbf{y})^T (\mathbf{X}\boldsymbol{w}-\mathbf{y})
  \end{align*}
  ](https://render.githubusercontent.com/render/math?math=%5CHuge+%5Ctextstyle+%5Cbegin%7Balign%2A%7D%0AR%28g%29+%26%3D+%5Cfrac%7B1%7D%7Bn%7D+%5Csum_%7Bi%3D1%7D%5E%7Bn%7D+%5Cell%28y_i%2Cg%28x_i%29%29%5C%5C%0A%26%3D%5Cfrac%7B1%7D%7B2n%7D+%28%5Cmathbf%7BX%7D%5Cboldsymbol%7Bw%7D-%5Cmathbf%7By%7D%29%5ET+%28%5Cmathbf%7BX%7D%5Cboldsymbol%7Bw%7D-%5Cmathbf%7By%7D%29%0A%5Cend%7Balign%2A%7D%0A)