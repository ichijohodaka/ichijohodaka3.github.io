
1. ファイル名をタップすると、例えばhtmlでエクスポートできる。
1. init_printing(use_unicode=True)でtex並の見栄えの数式で出力される
1. マークダウンモードでは、$で囲むとインライン数式、$$で改行して囲むと別行だての数式。円マークはそのまま出力される。オプションキーを押しながら、円マークキーを押すと、バックスラッシュが出て、これがtexのエスケープになる。




```python
from sympy import *
init_printing(use_unicode=True)
```


```python
x, y, A, B = symbols('x,y,A,B')
A = x**3 + 2 * x**2 * y - y**3
B = 3 * x**3 - x**2 * y + 3 * x * y**2 + 2 * y**3
A
B
```




$\displaystyle 3 x^{3} - x^{2} y + 3 x y^{2} + 2 y^{3}$




```python
3 * A + 2 * B - ( A + B )
```




$\displaystyle 5 x^{3} + 3 x^{2} y + 3 x y^{2}$




```python
B
```




$\displaystyle 3 x^{3} - x^{2} y + 3 x y^{2} + 2 y^{3}$




```python

```
