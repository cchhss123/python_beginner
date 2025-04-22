# 單元 3：判斷式與迴圈

本單元將介紹如何在 Python 中使用判斷式（`if`、`elif`、`else`）來根據條件執行不同的程式碼區塊，以及如何使用迴圈（`for`、`while`）來重複執行特定的程式碼。

## 判斷式 (`if`, `elif`, `else`)

判斷式用於根據條件的真假來決定要執行的程式碼。

* **`if` 語句：** 如果條件為真 (`True`)，則執行 `if` 區塊中的程式碼。
* **`elif` 語句：** (else if 的縮寫) 如果前一個 `if` 或 `elif` 的條件為假 (`False`)，則檢查 `elif` 的條件。如果 `elif` 的條件為真，則執行 `elif` 區塊中的程式碼。可以有多個 `elif` 語句。
* **`else` 語句：** 如果前面所有的 `if` 和 `elif` 的條件都為假 (`False`)，則執行 `else` 區塊中的程式碼。`else` 語句是可選的。

## 迴圈 (`for`, `while`)

迴圈用於重複執行一段程式碼，直到滿足特定條件為止。

* **`for` 迴圈：** 通常用於遍歷一個序列（例如：列表、字串、範圍等）中的每個元素。
* **`while` 迴圈：** 只要條件為真 (`True`)，就持續執行迴圈中的程式碼。需要小心確保迴圈最終會停止，避免無限迴圈。

## 範例程式碼

### #if, elif, else 判斷式
```python
score = 75

if score >= 90:
    grade = "A"
elif score >= 80:
    grade = "B"
elif score >= 70:
    grade = "C"
elif score >= 60:
    grade = "D"
else:
    grade = "F"

print(f"分數 {score} 對應的等級是 {grade}")
```

### #for 迴圈
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)

for i in range(5):  # range(5) 會產生 0, 1, 2, 3, 4 的序列
    print(f"數字: {i}")
```

### #while 迴圈
```python
count = 0
while count < 5:
    print(f"Count is: {count}")
    count = count + 1
```