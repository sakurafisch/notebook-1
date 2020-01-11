# Go语言笔记：语句

## 顺序语句

### `defer`

`defer`语句使后面的函数推迟到外层函数结束后调用；但函数的参数会被立即求值。

注意如果存在多条`defer`语句，则后面的`defer`语句会先执行。（后进先出顺序）

## 分支语句

### `if`

可在`if`的条件表达式前执行一个简单语句（就像`for`语句中的第一部分），简单语句中声明的变量的作用域在`if-else`语句块中可用。

### `switch`

1. `case`无需为常量，取值不必为整数。`switch`是书写多条`if`语句的清晰方式。
2. 无需提供`break`语句，除非以`fallthrough`语句结尾，否则分支会自动终止。
3. 从上而下顺次执行，直到匹配成功为止。
4. 无条件的`switch`相当于`switch true`，能将一连串的if-else-then写得更简洁。

## 循环语句

### `for`

只使用`for`循环。C语言中的`while`在Go中为`for`。

`for`语句的三部分由`;`隔开，花括号是必须的。

无限循环可简写为`for {}`。