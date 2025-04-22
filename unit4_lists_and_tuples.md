# 單元 4：串列與元組

本單元將深入介紹 Python 中的兩種重要的序列型資料結構：串列（list）和元組（tuple）。

## 串列 (list)

串列是一個**有序**且**可變**的元素集合。串列中的元素可以是不同的資料型態，並使用方括號 `[]` 包圍，元素之間用逗號 `,` 分隔。

### 串列的常用操作

* **建立串列：**
    ```python
    my_list = [1, 2, "hello", 3.14, True]
    empty_list = []
    ```
* **存取元素：** 使用索引（從 0 開始）來存取串列中的元素。
    ```python
    print(my_list[0])  # 輸出 1
    print(my_list[2])  # 輸出 hello
    print(my_list[-1]) # 輸出 True (最後一個元素)
    ```
* **切片 (slicing)：** 取得串列的子集合。
    ```python
    print(my_list[1:4])  # 輸出 [2, 'hello', 3.14]
    print(my_list[:3])   # 輸出 [1, 2, 'hello']
    print(my_list[2:])   # 輸出 ['hello', 3.14, True]
    ```
* **修改元素：** 因為串列是可變的，所以可以修改串列中的元素。
    ```python
    my_list[0] = 100
    print(my_list)  # 輸出 [100, 2, 'hello', 3.14, True]
    ```
* **新增元素：**
    * `append(element)`: 在串列末尾新增一個元素。
    * `insert(index, element)`: 在指定的索引位置插入一個元素。
    * `extend(iterable)`: 將另一個可迭代物件（例如：另一個串列）的所有元素新增到串列末尾。
* **刪除元素：**
    * `del my_list[index]`: 刪除指定索引位置的元素。
    * `remove(value)`: 刪除第一個匹配指定值的元素。
    * `pop(index)`: 刪除並返回指定索引位置的元素（如果沒有指定索引，則刪除並返回最後一個元素）。
* **其他常用方法：** `len()`（取得長度）、`count(value)`（計算元素出現次數）、`index(value)`（尋找元素索引）、`sort()`（排序）、`reverse()`（反轉）。

## 元組 (tuple)

元組是一個**有序**且**不可變**的元素集合。元組中的元素可以是不同的資料型態，並使用圓括號 `()` 包圍，元素之間用逗號 `,` 分隔。

### 元組的特性

* **不可變性：** 元組一旦建立後，就不能修改、新增或刪除其中的元素。
* **通常用於儲存不應該被修改的資料。**
* **在某些情況下比串列更有效率。**

### 元組的常用操作

* **建立元組：**
    ```python
    my_tuple = (1, 2, "hello", 3.14, True)
    empty_tuple = ()
    single_element_tuple = (5,)  # 注意單元素元組後面的逗號
    ```
* **存取元素和切片：** 與串列的操作方式相同。
    ```python
    print(my_tuple[0])  # 輸出 1
    print(my_tuple[1:3]) # 輸出 (2, 'hello')
    ```
* **由於元組是不可變的，因此沒有修改、新增或刪除元素的方法。**
* **其他常用方法：** `len()`（取得長度）、`count(value)`（計算元素出現次數）、`index(value)`（尋找元素索引）。

## 範例程式碼

### #串列範例
```python
numbers = [10, 20, 30, 40, 50]
print(f"原始串列: {numbers}")

numbers[2] = 35
print(f"修改後的串列: {numbers}")

numbers.append(60)
print(f"新增元素後的串列: {numbers}")

numbers.insert(1, 15)
print(f"插入元素後的串列: {numbers}")

del numbers[0]
print(f"刪除第一個元素後的串列: {numbers}")

print(f"串列長度: {len(numbers)}")
print(f"元素 35 出現的次數: {numbers.count(35)}")
```

### #元組範例
```python
point = (3, 5)
print(f"座標: {point}")
print(f"x 座標: {point[0]}")
print(f"y 座標: {point[1]}")

# point[0] = 10  # 這行會報錯，因為元組是不可變的

dimensions = (1920, 1080)
print(f"解析度: {dimensions}")
print(f"寬度: {dimensions[0]}")
print(f"高度: {dimensions[1]}")
```