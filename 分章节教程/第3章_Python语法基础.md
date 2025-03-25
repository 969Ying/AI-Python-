# 第3章 Python语法基础

## 知识目标
- 掌握Python的基本语法结构
- 理解Python中的数据类型和运算符
- 学会使用控制结构和函数进行编程

## 理论详解
### 变量与数据类型
- **变量**：用于存储数据的命名空间。
- **数据类型**：
  - **基本数据类型**：整数（int）、浮点数（float）、字符串（str）
  - **复杂数据类型**：列表（list）、字典（dict）、元组（tuple）

### 运算符
- **算术运算符**：`+`, `-`, `*`, `/`, `//`, `%`, `**`
- **比较运算符**：`==`, `!=`, `>`, `<`, `>=`, `<=`
- **逻辑运算符**：`and`, `or`, `not`

### 控制结构
- **条件语句**：`if`, `elif`, `else`
- **循环语句**：`for`, `while`

## 操作指南
### Python基本语法使用
1. **定义变量**：
   ```python
   x = 10
   y = 3.14
   name = "Alice"
   ```
2. **使用运算符**：
   ```python
   result = x + y
   is_equal = (x == 10)
   ```
3. **控制结构**：
   ```python
   if x > 5:
       print("x is greater than 5")
   else:
       print("x is less than or equal to 5")
   ```

## 代码示例
### 使用函数进行简单计算
```python
def calculate_total(revenues):
    # 计算总收入
    total = sum(revenues)
    return total

# 示例数据
revenues = [1000, 1500, 2000]
total_revenue = calculate_total(revenues)
print(f"Total Revenue: {total_revenue}")
```
**输出说明**：该代码定义了一个函数用于计算总收入，并输出结果。

## 财务实践
- **数据处理**：使用Python进行数据的增删改查。
- **自动化计算**：编写脚本自动计算财务指标。

## 常见问题
1. **语法错误**：
   - **解决方案**：检查代码缩进和语法格式，确保符合Python语法规则。

2. **数据类型错误**：
   - **解决方案**：使用`type()`函数检查变量类型，确保操作的数据类型匹配。

3. **循环或条件语句错误**：
   - **解决方案**：检查循环和条件语句的逻辑，确保条件判断正确。

## 3.1 变量
- **变量的定义与使用**：变量是用于存储数据的命名空间，可以通过赋值语句进行定义和使用。
  ```python
  x = 10
  y = "Hello"
  ```
- **变量命名规则**：变量名必须以字母或下划线开头，后续可以包含字母、数字和下划线，区分大小写。
  ```python
  my_variable = 5
  _hidden_value = 42
  ```

## 3.2 注释
- **单行注释与多行注释**：单行注释使用`#`，多行注释使用三个引号`'''`或`"""`。
  ```python
  # 这是一个单行注释
  """
  这是一个
  多行注释
  """
  ```
- **注释的最佳实践**：注释应简洁明了，解释代码的目的和逻辑，而不是逐行翻译代码。

## 3.3 数据类型
- **基本数据类型**：
  - **整数（int）**：用于表示整数值。
  - **浮点数（float）**：用于表示小数。
  - **字符串（str）**：用于表示文本。
  ```python
  age = 30
  height = 5.9
  name = "Alice"
  ```
- **复杂数据类型**：
  - **列表（list）**：有序可变集合。
  - **字典（dict）**：键值对集合。
  - **元组（tuple）**：有序不可变集合。
  ```python
  fruits = ["apple", "banana", "cherry"]
  person = {"name": "Alice", "age": 30}
  coordinates = (10.0, 20.0)
  ```

## 3.4 运算符
- **算术运算符**：用于数学计算，如`+`, `-`, `*`, `/`, `//`, `%`, `**`。
  ```python
  sum = 5 + 3
  product = 4 * 2
  ```
- **比较运算符**：用于比较值，如`==`, `!=`, `>`, `<`, `>=`, `<=`。
  ```python
  is_equal = (5 == 5)
  is_greater = (10 > 5)
  ```
- **逻辑运算符**：用于逻辑运算，如`and`, `or`, `not`。
  ```python
  result = (5 > 3) and (2 < 4)
  ```

## 3.5 控制结构
- **条件语句**：用于根据条件执行代码块。
  ```python
  if x > 0:
      print("x is positive")
  elif x == 0:
      print("x is zero")
  else:
      print("x is negative")
  ```
- **循环语句**：用于重复执行代码块。
  ```python
  for i in range(5):
      print(i)
  
  while x > 0:
      x -= 1
  ```

## 3.6 函数
- **函数的定义与调用**：函数是可重用的代码块，通过`def`关键字定义。
  ```python
  def greet(name):
      return f"Hello, {name}!"
  
  print(greet("Alice"))
  ```
- **参数与返回值**：函数可以接收参数并返回值。
  ```python
  def add(a, b):
      return a + b
  
  result = add(3, 4)
  ```

## 3.7 模块
- **模块的导入与使用**：模块是包含Python代码的文件，可以通过`import`导入。
  ```python
  import math
  print(math.sqrt(16))
  ```
- **常用内置模块**：如`os`, `sys`, `datetime`等。

## 3.8 异常
- **异常的捕获与处理**：使用`try`和`except`处理异常。
  ```python
  try:
      result = 10 / 0
  except ZeroDivisionError:
      print("Cannot divide by zero")
  ```
- **自定义异常**：可以通过继承`Exception`类创建自定义异常。
  ```python
  class CustomError(Exception):
      pass
  ``` 