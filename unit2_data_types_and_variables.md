# 單元 2：資料型態與變數

本單元將介紹 Python 中常用的資料型態以及如何使用變數。

## 資料型態

* **整數 (int)：** 表示沒有小數點的數字，例如：`10`、`-5`。
* **浮點數 (float)：** 表示帶有小數點的數字，例如：`3.14`、`-2.5`。
* **字串 (str)：** 表示一串文字，用單引號 `' '` 或雙引號 `" "` 包圍，例如：`'Hello'`、`"Python"`。
* **布林值 (bool)：** 表示真或假，只有兩個值：`True` 和 `False`。

## 變數

變數是用來儲存資料的名稱或代號(未知數)。在 Python 中，您可以直接賦值來建立變數，不需要事先宣告資料型態。

### 變數命名規則

* 變數名稱只能包含字母、數字和底線 (`_`)。
* 變數名稱不能以數字開頭。
* 變數名稱區分大小寫（例如：`myVariable` 和 `myvariable` 是不同的）。
* 避免使用 Python 的保留字（例如：`print`、`if`、`for` 等）作為變數名稱。
* 建議使用具有描述性的變數名稱，以提高程式碼的可讀性。

## 範例程式碼

```python
# 整數
age = 30
print(f"我的年齡是: {age}, 型別是: {type(age)}")

# 浮點數
pi = 3.14159
print(f"圓周率是: {pi}, 型別是: {type(pi)}")

# 字串
name = "Alice"
print(f"我的名字是: {name}, 型別是: {type(name)}")

message = '歡迎來到 Python 的世界！'
print(f"訊息: {message}, 型別是: {type(message)}")

# 布林值
is_student = False
print(f"我是學生嗎？{is_student}, 型別是: {type(is_student)}")

# 變數賦值與修改
count = 0
print(f"初始計數: {count}")
count = count + 1
print(f"計數加一後: {count}")
```