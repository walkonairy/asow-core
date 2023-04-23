### 什么是闭包？
闭包其实就是一个可以访问其他函数内部变量的函数。创建闭包的最常见的方式就是在一个函数内创建另一个函数，创建的函数可以访问到当前函数的局部变量。    

#### 本质（产生原因）
作用域链的一个特殊的应用, 即当前环境中存在指向父级作用域的引用

#### 用途   
- 使我们在函数外部能够访问到函数内部的变量。我们可以通过在外部调用闭包函数，从而在外部访问到函数内部的变量，可以使用这种方法来创建私有变量
- 使已经运行结束的函数上下文中的变量对象继续留在内存中，因为闭包函数保留了这个变量对象的引用，所以这个变量对象不会被回收。

#### 表现形式
- 返回一个函数
- 回调函数
- 作为函数参数传递