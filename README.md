# プログラミング2021 期末試験 模範解答

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
x = [x] * 2
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

## Q13  (5点)

次のPythonコードを実行したあと、続けて実行したときにエラーが出ないコードには○を、エラーが出るコードには☓をつけなさい。

```python
x = {'a':1,'b':2,'c':3}
```

1. `x[[1,2]] = 'a'`
2. `x[1] = 'a'`
3. `x[{1,2,3}] = 'a'`
4. `y = x[0]`
5. `del x['b']`

## Q14 (2点)

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = {'a':2,'a':4,'b':6}
x.update({'b':7,'b':13})
print(x['a'] + x['b'])
```

## Q15 (2点)

次のコードを実行した結果出力されるリストを記述しなさい（例：[1,2,3]）。

```python
x = [1,1,2,2,3,3]
y = [3,4,5,5]
y = list(set(x).union(set(y)))
print(y)
```

## Q16

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(10):
    if i % 3 == 0:
        x += 1
    elif i % 2 == 0:
        x -= 1
print(x)
```

答え：1

## Q23 (5)

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(10):
    if i % 3 == 0:
        x += 1
    if i % 2 == 0:
        x -= 1
print(x)
```

答え：-1

## Q24 (5)

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(10):
    if i % 3 == 0:
        x += 1
        if i % 2 == 0:
            x -= 1
print(x)
```

答え：2

## Q25 (5)

次のPythonコードを実行した結果出力される整数を答えなさい。

```python
x = 0
for i in range(5):
    for j in range(0,i):
        x += 1
    x -=1
print(x)
```

答え：5


## Q33 (5)

次のPythonコードを実行した際に得られる出力を整数値で答えなさい。ただし64ビット処理系を仮定する。

```python
import sys
x = dict()
for i in range(0,5):
    x[i] = i
overhead = sys.getsizeof(dict()) - 128
print(sys.getsizeof(x)-overhead)
```

答え：128

## Q35 (各1計4)

次のPythonコードを実行したとします。

```python
x = {'dog','cat','horse'}
y = {'cow'}.union(x)
z = x.intersection({'cat','horse','sheep'})
```

次のうち、TrueになるものにはT、FalseになるものにはFと答えなさい。(部分点あり)

1. `z.issuperset(x)` F
2. `x.issubset(y)` T
3. `z.issubset(y)` T
4. `z in y` F

## Q36 (各1計6)

次のPythonコードのうち、エラーが出ずに実行できるものには○を、そうでないものには☓をつけなさい。（部分点あり）

1. `{[],()}` ×
2. `{{(0)}}` ×
3. `{'':[]}` ○
4. `{():dict()}` ○
5. `{([],):1}` ×
6. `dict(5='a')` ×

## Q37 (5)

次のPythonコードを実行した際に出力される整数を書きなさい。

```python
print({i % 4:i for i in range(10)}[0])
```

答え：8

## Q38 (4)

次のコードを実行したとき、`x`には何が代入されているか答えなさい。

```python
def func(x):
  if x > 1:
    return
  return x

x = func(2)
```

答え：`None`

## Q39 (5)

次のPythonコードを実行した際に、`x`に格納されているリストを記述しなさい。例:`[1,2,3,4]`

```python
def generator():
  x = 1
  for i in range(2,7):
    yield x
    x *= i

gen = generator()

x = list(gen)
```

答え：`[1,2,6,24,120]`

## Q40 (5)

次のPythonコードを実行した際に出力される整数を答えなさい。

```python
x = range(10)
y = [i if i%2==0 else -i for i in x if i % 3 != 0]
print(y[3])
```

答え：-5

## Q41 (5)

次のPythonコードは100以下の全ての素数を出力するためのコードです。(a)-(c)に当てはまるコードを1~4から選びなさい。

```python
for i in range(2,100):
  for j in range(2,i):
    (a)______
      (b)_____
  else:
    (c)______
```

1. `print(i)`
2. `break`
3. `continue`
4. `if i % j == 0`

答え：(a)4,(b)2,(c)1

## Q42 (5)

次のPythonコードは、"My teacher is a crazy guy."という文字列に含まれる各アルファベットの出現回数を印字するものである(大文字と小文字は区別しない)。

```python
string = 'My teacher is a crazy guy.'
trans_rule = {' ':'','.':''}
trans = str.maketrans(trans_rule)
sclean = string.lower().translate(trans)
x = dict()
for c in (a)_____:
  if c in (b)_____:
    x[c] += 1
  else:
    x[c] = 1
for k in sorted(x):
  print("{}/{}".format(k,x[k]))
```

出力は次のようになります。

```bash
a/3
c/2
e/2
g/1
h/1
i/1
m/1
r/2
s/1
t/1
u/1
y/3
z/1
```

(a)-(b)に当てはまる正しいコードを次から選びなさい。

1. `x.items()`
2. `sclean`
3. `set(sclean)`
4. `x.keys()`

答え：(a)2,(b)4
