# プログラミング2023 期末試験

丸かっこ内の数字は配点です。

## Q1 (6点)

次の質問に答えなさい。

1. 32GiBは何MiBですか？
2. 32GBは何MBですか？
3. 1MiBと1MBの間には何バイトの差がありますか？

## Q2 (6点)

次のうち、正しい記述には○を、誤った記述には×をつけなさい。

1. コンパイルは不可逆変換である。
2. Pythonはコンパイル型言語である。
3. マシン語からアセンブリ言語のコードを生成することを逆アセンブルと呼ぶ。
4. メモリの情報を読み書きする際の単位は1ビットである。
5. アセンブリ言語によるコーディングでは、CPUのレジスタを直接操作する必要がある。
6. ソースコードからマシン語を生成するプロセスをバイトコンパイルと呼ぶ。

## Q3 (6点)

以下の問に答えなさい。

1. 16進数の4bを10進数で表記しなさい。
2. 10進数の200を2進数で表記しなさい。
3. 2進数の101011を16進数で表記しなさい。

## Q4 (2点)

次のPythonコードを実行したときに得られる出力として正しいものを一つ選びなさい。

```python
x = [1,2,3]
y = x
y[1] = 4
print(x,x is y)
```

1. `[1,2,3] True`
2. `[1,2,3] False`
3. `[1,4,3] True`
4. `[1,4,3] False`

<div style="page-break-before:always"></div>

## Q5 (2点)

次のPythonコードを実行したときに得られる出力として正しいものを一つ選びなさい。

```python
x = [1,2,3]
y = x[:]
y[1] = 4
print(x,x is y)
```

1. `[1,2,3] True`
2. `[1,2,3] False`
3. `[1,4,3] True`
4. `[1,4,3] False`

## Q6 (2点)

次のPythonコードを実行したときに得られる出力として正しいものを一つ選びなさい。

```python
x = [1,2,3,4]
y = x[1:3]
print(y)
```

1. `[1,2,3]`
2. `[2,3,4]`
3. `[2,3]`
4. `[1,2,3,4]`

## Q7 (8点)

次のPythonコードを実行したあと、続けて実行したときにエラーが出ないコードには○を、エラーが出るコードには☓をつけなさい。

```python
x = "computer"
```

1. `x[:] == 'program'`
2. `x[:3] = "COM"`
3. `y = "personal " + x`
4. `y = x[3:7]`
5. `x = "python"`
6. `x = x + 1`
7. `y = 2 * x + 3 * x`
8. `y = 3 * x - 2 * x`

<div style="page-break-before:always"></div>

## Q8 (2点)

次のPythonコードを実行したときに得られる出力として正しいものを一つ選びなさい。

```python
x = ['foo',['bar'],'baz']
y = x.copy()
x[1][0] = 'py'
print(y,x is y)
```

1. `['foo',['py'],'baz'] True`
2. `['foo',['py'],'baz'] False`
3. `['foo',['bar'],'baz'] True`
4. `['foo',['bar'],'baz'] False`

## Q9 (2点)

次のPythonコードを実行した結果得られる出力として正しいものを一つ選びなさい。

```python
x = [[1,2]]
x = x * 2
x[0][0] = 3
print(x)
```

1. `[3,2,1,2]`
2. `[[3,2],[1,2]]`
3. `[[3,2],[3,2]]`
4. `[3,2,3,2]`

## Q10  (4点)

次のうち、Pythonのタプルであるものには○を、そうでないものには☓をつけなさい。

1. `(,)`
2. `(1,)`
3. `()`
4. `(1)`

<div style="page-break-before:always"></div>

## Q11  (5点)

次のPythonコードを実行したあと、続けて実行したときにエラーが出ないコードには○を、エラーが出るコードには☓をつけなさい。

```python
x = (1,2,[3])
```

1. `x[0] = 4`
2. `y = x + (4,5,6)`
3. `y = x * 3`
4. `x[2] = [4]`
5. `x[2][0] = 4`

## Q12 (2点)

次のPythonコードを実行した結果出力として得られる文字列を答えなさい。解答例：`abCDefg`

```python
trans_rule = {'a':'b','c':'d'}
trans = str.maketrans(trans_rule)
print("abcdabcd".translate(trans))
```

## Q13  (6点)

次のPythonコードを実行したあと、続けて実行したときにエラーが出ないコードには○を、エラーが出るコードには☓をつけなさい。

```python
x = {'a':1,'b':2,'c':3}
```

1. `x[[1,2]] = 'a'`
2. `x[1] = 'a'`
3. `x[{1,2,3}] = 'a'`
4. `y = x[0]`
5. `x[(1,[])] = 4`
6. `x[()] = 4`

## Q14 (2点)

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = {'a':2,'a':4,'b':6}
x.update({'b':7,'b':13})
print(x['a'] + x['b'])
```

<div style="page-break-before:always"></div>

## Q15 (2点)

次のコードを実行した結果出力されるリストを記述しなさい（例：[1,2,3]）。

```python
x = [1,1,2,2,3,3]
y = [3,4,5,5]
y = list(set(x).union(set(y)))
print(y)
```

## Q16  (2点)

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(10):
    if i % 3 == 0:
        x += 1
print(x)
```

## Q17  (2点)

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(10):
    if i % 3 == 0:
        x += 1
        if i % 2 == 0:
            x += 2
print(x)
```

## Q18 (2点)

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(10):
    if i % 3 == 0:
        x += 1
    if i % 2 == 0:
        x += 2
print(x)
```

<div style="page-break-before:always"></div>

## Q19 (2点)

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(10):
    if i % 3 == 0:
        x += 1
    elif i % 2 == 0:
        x += 2
print(x)
```

## Q20 (3点)

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(5):
    x += i
    for j in range(i+1):
        x += j
print(x)
```

## Q21 (2点)

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 100
while x % 13 != 0:
  x -= 1

print(x)
```

## Q22  (3点)

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 1
for i in range(10):
  x += i
  if x > 50:
    break
else:
  x += 3

print(x)
```

<div style="page-break-before:always"></div>

## Q23 (2点)

次のPythonコードを実行した際に出力される整数を書きなさい。

```python
x = [i*2 for i in range(10) if i % 2 == 0]
print(x[3])
```

## Q24 (1点)

次のコードを実行したとき、`x`には何が代入されているか答えなさい。

```python
def func():
  return

x = func()
```

## Q25 (3点)

次のコードを実行したときに出力される整数を答えなさい。

```python
def func(x):
  y = x
  if y > 1:
    y += func(y-1)
  return y

x = func(4)
print(x)
```

## Q26  (3点)

次のPythonコードを実行したときに出力される整数を答えなさい。

```python
def generator(n):
  x = 1
  while True:
    yield x**n
    x += 1

gen = generator(3)

x = [next(gen)-i for i in range(5)]
print(x[3])
```

<div style="page-break-before:always"></div>

## Q27  (5点)

Pythonに関する以下の記述の内、正しいものには○を、誤っているものには☓をつけなさい。

1. 関数の中で値を代入された変数はグローバル名前空間に属する
2. ビルトインスコープはプログラム全体である。
3. ビルトインモジュールにはbuiltinsモジュールの他に、sysモジュールやmathモジュールなどがある。
4. モジュールは、原則としてバイトコンパイルされない。
5. Pythonの再起動なしに、一度読み込んだモジュールをimport文で再度読み込むことはできない。

## Q28  (2点)

次のPythonコードを実行したときに出力される整数を答えなさい。

```python
x = 0
def f():
    x = 1
    def g():
        print(x)
    g()
f()
```

## Q29  (3点)

次のPythonコードを実行したときに出力される整数を答えなさい。

```python
def outer():
    y = 0
    def inner(x):
        nonlocal y
        y += x
        return y
    return inner
cl = outer()
x = [cl(i) for i in range(5)]
print(x[-1])
```

## Q30 (2点)

次のPythonコードを実行したときに出力される整数を答えなさい。

```python
import numpy as np
x = np.arange(10)
x += 3
print(x[5])
```

<div style="page-break-before:always"></div>

## Q31 (2点)

次のPythonコードを実行したときに出力される整数を答えなさい。

```python
import numpy as np
x = np.array([2,3,5])
y = np.array([1,9,4])
z = x * y
print(z[1])
```

## Q32  (2点)

次のPythonコードを実行したときに出力される整数を答えなさい。

```python
import numpy as np
x = np.arange(10)
y = x[3:8:2]
x += 5
print(y[1])
```

## Q33  (2点)

以下のPythonコードは、Numpyを用いて、切片5、傾き2の線形モデルに従うサンプルサイズ100の疑似データを生成し、変数yに配列として格納するためのものである。ただし実測値yは標準正規分布に従う誤差を含むとする。#????に書くべきコードを答えなさい。

```python
import numpy as np
x = np.random.normal(5,2,100)
e = np.random.normal(0,1,100)
y = #????
```
