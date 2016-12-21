## deletechannel

### 概要

从内存中的文件列表中删除一个或多个文件

### 语法

``` {.bash}
DELETECHANNEL ALL
```
``` {.bash}
DC ALL
```

或

``` {.bash}
DELETECHANNEL fname|fno|range [fname|fno|range ...]
```
``` {.bash}
DC fname|fno|range [fname|fno|range ...]
```

### 输入

- `ALL`: 删除内存中全部文件
- `fname`: 要删除文件的文件名
- `filenumber`: 要删除文件的文件号。第一个文件的文件号是1
- `range`: 要删除文件的文件号范围，范围用破折号分开，如`11-20`

### 示例

``` {.bash}
  dc 3 5                         // 删除第3、5个文件
  dc SO01.sz SO02.sz             // 删除这些名字的文件
  dc 11-20                       // 删除第11至20个文件
  dc 3 5 11-20 SO01.sz SO02.sz   // 删除上面的全部文件
```