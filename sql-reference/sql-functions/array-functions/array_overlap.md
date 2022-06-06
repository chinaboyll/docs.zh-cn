# arrays_overlap

## 功能

判断两个相同类型的数组中是否包含相同的元素。返回`1`代表存在相同元素，返回`0`代表不存在相同元素。

## 语法

```Haskell
output arrays_overlap(input0, input1)
```

## 参数说明

* `input0`：数组。
* `input1`: 与`input0`类型一致的数组。

## 返回值说明

返回 BOOLEAN 类型的数值。

## 示例

**示例一**

```plain text
mysql> select arrays_overlap([11, 9, 3, 2], [null, 11]);
+--------------------------------------+
| arrays_overlap([11,9,3,2], [NULL,11]) |
+--------------------------------------+
|                                    1 |
+--------------------------------------+
```

**示例二**

```plain text
mysql> select arrays_overlap([9, 3, 2], [null, 11]);
+-----------------------------------+
| arrays_overlap([9,3,2], [NULL,11]) |
+-----------------------------------+
|                                 0 |
+-----------------------------------+
```

**示例三**

```plain text
mysql> select arrays_overlap([9, 3, null, 2], [null, 11]);
+----------------------------------------+
| arrays_overlap([9,3,NULL,2], [NULL,11]) |
+----------------------------------------+
|                                      1 |
+----------------------------------------+
```

**示例四**

```plain text
mysql> select arrays_overlap([9, 3, "SQL", 2], [null, "SQL"]);
+--------------------------------------------+
| arrays_overlap([9,3,'SQL',2], [NULL,'SQL']) |
+--------------------------------------------+
|                                          1 |
+--------------------------------------------+
```

## 关键词

ARRAYS_OVERLAP