# Shell 数组

Bash Shell 只支持一维数组（不支持多维数组），初始化时不需要定义数组大小。数组元素的下标由0开始。

Shell 数组用括号来表示，元素用"空格"符号分割开，语法格式如下：

```shell
array_name=(value1 ... valuen)
```

**实例**

```shell
#!/bin/bash
my_array=(A B "C" D)
```

也可以使用下标来定义数组:

```shell
array_name[0]=value0
array_name[1]=value1
array_name[2]=value2
```

**读取数组**

读取数组的一般格式为：

```shell
${array_name[index]}
```

**获取数组中的所有元素**

使用@ 或 * 可以获取数组中的所有元素，例如：

```shell
#!/bin/bash

my_array[0]=A
my_array[1]=B
my_array[2]=C
my_array[3]=D

echo "数组的元素为: ${my_array[*]}"
echo "数组的元素为: ${my_array[@]}"
```

**获取数组的长度**

获取数组长度的方法与获取字符串长度的方法相同，例如：

```shell
#!/bin/bash

my_array[0]=A
my_array[1]=B
my_array[2]=C
my_array[3]=D

echo "数组元素个数为: ${#my_array[*]}"
echo "数组元素个数为: ${#my_array[@]}"
```

