# 道语言：传统智慧与现代技术的完美融合
道语言，不仅是连接传统与现代的桥梁，更是创新与传承的交汇点。汉语，作为中华民族的文化瑰宝、灵魂所在、文明标志，以其非凡的信息压缩技艺，在世界语言之林中独树一帜。举例而言，“中华人民共和国”这一庄严国名，在英语中需29个字母方能完整表达，而中文仅以四个字便足以精确传达，甚至可进一步简化为“中国”，或仅用“中”与“华”一字以蔽之。这种极致的凝练，正是中文魅力的独特体现。

追溯至文言文的黄金时代，其文字之精炼，达到了无以复加的境界。每一个字都如同一颗珍贵的宝石，不多添一笔，不少去一划，却能将深奥复杂的意境表达得清晰透彻。这一传统激发了我们的灵感：能否将文言文的精华，融合现代科技，创造出一门全新的编程语言？这不仅是对中华文化瑰宝的传承，也是与现代计算机技术相结合，以提高开发效率的创新探索。我们致力于打造一门既优雅又高效的编程语言——道语言��全球见证中华文化的深邃与智慧。

秉承“大道至简”的哲学精神，我们追求以最简练的文字承载最丰富的意义，简约而不失优雅。我们不仅继承传统，更融入现代符号的简洁性，博采众长，创造出一门全新的语言，我们称之为“道”。道语言，正是这一理念的生动实践，它将引领编程领域进入一个全新的时代，为中华文化续写辉煌的新篇章。

# **开放申明**
  **本语言设计为开源语言，目前暂是构建中文编程语言的语法规范，本人在这抛砖引玉，欢迎同志道合的朋友一起参与进来，给出改建建议，共同完善和发展。希望无论是系统级语言、还是解析性语言的建设，都非常欢迎使用这套标准**

# 设计目标
  本语言设计目标为：
  1. 精简语法，提高开发效率
  2. 传承中华文化，弘扬中华文明
  3. 融合现代技术，提高开发效率

# 设计原则
  1. 关键字优先使用单字
  2. 保留必要空格，提升可读性
  3. 省略非必要符号

# 特性说明

1. **简约原则**：
   - 关键字优先使用单字
   - 保留必要空格，提升可读性
   - 省略非必要符号

2. **命名建议**：
   - 变量名推荐使用单字或双字
   - 函数名应简明扼要
   - 注释使用文言文风格

3. **符号使用**：
   - 严格使用规定的运算符号和比较符号
   - 保持与现代编程语言的符号习惯一致
   - 数字统一使用阿拉伯数字


# 语法设计

## 一、符号系统

### 1. 运算符号
  
- 算术运算：`+`（加）、`-`（减）、`*`（乘）、`/`（除）
- 赋值运算：`=`（赋值）
- 括号：`(`（左括号）、`)`（右括号）
- 数字：使用阿拉伯数字（0-9）

### 2. 比较符号
- 大于：`>`
- 小于：`<`
- 大于等于：`>=`
- 小于等于：`<=`
- 等于：`==`
- 不等于：`!=`

## 二、基础语法

### 1. 变量声明与赋值
- 公共变量：`宣`  // 显式声明为全局变量
- 常量：`恒`      // 显式声明为常量
- 局部变量：直接声明，无需关键字  // 移除 '域' 关键字

示例：
```go
宣 数 整 = 10    // 全局变量
恒 圆周率 浮 = 3.14159  // 常量
计 整 = 0        // 局部变量，省略'域'字
```

### 2. 基本类型
- 整数：`整` 另外整数又有int、int8、int16、int32、int64、uint、uint8、uint16、uint32、uint64、uintptr,分别用`整`、`整8`、`整16`、`整32`、`整64`、`无整`、`无整8`、`无整16`、`无整32`、`无整64`、`无整指针`表示
- 浮点：`浮` 另外浮点又有float32、float64,分别用`浮32`、`浮64`表示
- 字符串：`串` 另外字符串又有string,用`串`表示
- 布尔：`判` 另外布尔又有bool,用`判`表示
- 复数：`复` 另外复数又有complex64、complex128,分别用`复64`、`复128`表示
- 空：`空`

### 3. 函数定义
- 函数：`术`
- 返回：`还`
- 参数：`入`

示例：
```go
术 加(甲 整, 乙 整) 整 {
    还 甲 + 乙
}
```

### 4. 流程控制
- 条件判断：`若`、`则`、`否`
- 循环：`循`
- 遍历：`历`
- 跳出：`出`
- 继续：`续`
- 多条件：`或`、`且`
- 分支选择：`择`、`其`、`默`  // switch、case、default

示例：
```go
若 数 大 0 则 {
    还 真
} 否 {
    还 伪
}

循 (计 小 10) {
    计 得 计 + 1
}

历 数组 元 {
    示 元
}

// 基本择语句  
择 值 {
    其 1:
        示("其一")
    其 2:
        示("其二")
    遂:      //来源 “余无所取，遂得此。”（我没有选择其他的，因此自然得到了这个。）
        示("其他")
}

// 带条件的择语句
择 {
    其 年 > 60:
        示("老年")
    其 年 > 30:
        示("中年")
    其 年 > 18:
        示("青年")
    默:
        示("少年")
}

// 类型择语句
择 值.(型) {
    其 整:
        示("整数")
    其 串:
        示("字符串")
    其 浮:
        示("浮点数")
    默:
        示("未知类型")
}
```

### 5. 数据结构
- 数组：`列`
- 切片：`段`
- 映射：`图`
- 结构：`体`
- 接口：`衔`

示例：
```go
宣 数列 列[5]整
宣 数段 段[]整
宣 字图 图[串]整

体 人 {
    名 串
    岁 整
}
```

### 6. 错误处理
- 错误：`误`
- 异常：`异`
- 延迟：`延`
- 恢复：`复`

示例：
```go
术 除(甲 整, 乙 整) (整, 误) {
    若 乙 等 0 则 {
        还 0, 新误("除数不可为零")
    }
    还 甲 / 乙, 空
}
```

### 7. 包管理类
- 包声���：`包`
- 导入包：`引`
- 公开成员：`公`
- 私有成员：`私`

### 8. 并发处理类
- 协程：`程`
- 通道：`通`
- 接收：`收`
- 发送：`发`
- 选择：`择`

示例：
```go
术 并发示例() {
    通 甲道 = 创通(整)
    通 乙道 = 创通(整)
    通 丙道 = 创通(整)

    程 函() {
        发 甲道 <- 1
    }

    程 函() {
        发 乙道 <- 2
    }

    择 {
        值 := <-收 甲道:
            示("收到甲道:", 值)
        值 := <-收 乙道:
            示("收到乙道:", 值)
        丙道 <- 3:
            示("发送至丙道")
        待 2 * 时.秒:
            示("超时")
    }
}
```

### 9. 逻辑运算类
- 与：`且`
- 或：`或`
- 非：`非`
- 真：`真`
- 伪：`伪`

### 10. 类型转换类
- 转换：`化`，如整转浮32：`整化浮32(整数1)`,如浮转整：`浮化整(浮数1)`，如整转无整：`整化无整(整数1)`，如无整转整：`无整化整(无整1)`，如浮转无浮：`浮化无浮(浮数1)`，无浮转浮：`无浮化浮(无浮1)` ，如时间转字符：`时间化串(时间1)`，如字符转时间：`串化时间(字符串1)`
- 断言：`断`
- 类型：`型` 

### 11. 集合与序列操作类
- 长度：`长`  // 获取长度
- 容量：`容`  // 获取容量
- 追加：`加`  // append 操作
- 截取：`截`  // slice 操作
- 复制：`复`  // copy 操作
- 删除：`删`  // delete 操作（用于 map）
- 创建：`创`  // make 操作

示例：
```go
// 切片操作
域 数段 = 创段(整, 0, 10)
加(数段, 1)
长度 := 长(数段)
容量 := 容(数段)
片段 := 截(数段, 1, 3)

// 映射操作
域 数图 = 创图(串, 整)
数图["甲"] = 1
删(数图, "甲")

// 复制操作
域 源段 = []整{1, 2, 3}
域 目段 = 创段(整, 3)
复(目段, 源段)
```

### 12. 文件操作类
- 读取：`读`
- 写入：`写`
- 打开：`开`
- 关闭：`闭`
- 创建：`创`

### 13. 时间处理类
- 等待：`待`
- 计时：`计`
- 超时：`超`

### 14. Go+ 特性支持
- 数据科学：`矩`（matrix，矩阵运算）
- 可选链：`选`（optional chaining）
- 范围：`界`（range）
- 列表推导：`导`（list comprehension）
- 泛型：`泛`（generics）

示例：

```go
// 矩阵运算
术 矩阵示例() {
    域 甲矩 = [[1, 2], [3, 4]]
    域 乙矩 = [[5, 6], [7, 8]]
    域 合矩 = 甲矩 + 乙矩
}

// 可选链
术 选链示例(物 *体) {
    域 值 = 物?.名?.长()
}

// 列表推导
术 列表示例() {
    域 数段 = [x*x : x <- 1:10]  // 1到10的平方
}

// 泛型
术 交换[甲 泛型](甲值, 乙值 甲) (甲, 甲) {
    还 乙值, 甲值
}
```

### 15. 科学计算支持
- 统计：`计`
- 绘图：`绘`
- 数据：`据`
- 分析：`析`

示例：
```go
术 科学计算() {
    // 统计计算
    域 均值 = 计.均([1, 2, 3, 4, 5])
    域 方差 = 计.方([1, 2, 3, 4, 5])
    
    // 数据可视化
    绘.线([1, 2, 3], [4, 5, 6])
    绘.显()
}
```

### 16. 脚本特性
- 命令执行：`令`
- 管道：`管`
- 重定向：`向`

示例：
```go
术 脚本示例() {
    // 执行系统命令
    域 输出 = 令("ls -l")
    
    // 管道操作
    域 结果 = 令("ls").管(令("grep .go"))
}
```

### 17. 指针操作
- 指针类型：`指`
- 取地址：`址`
- 取值：`值`

示例：
```go
// 基本指针操作
甲 整 = 100
乙 指整 = 址甲      // 取甲的地址
值乙++              // 通过指针修改值
示(甲)             // 输出 101

// 指向指针的指针
甲 整 = 100
乙 指整 = 址甲
丙 指指整 = 址乙
示(甲)             // 输出 100
示(值乙)           // 输出 100
示(值值丙)         // 输出 100

// 空指针
空指 指整          // 声明空指针
若 空指 == 空 {
    示("空指针")
}

// 结构体指针
体 人 {
    名 串
    岁 整
}

术 改名(人指 指人, 新名 串) {
    人指.名 = 新名    // 通过指针修改结构体字段
}

// 使用示例
某人 人 = 人{名: "张三", 岁: 20}
改名(址某人, "李四")
示(某人.名)          // 输出 "李四"
```

指针操作说明：
1. 使用`指`表示指针类型，如`指整`表示整数指针
2. 使用`址`获取变量地址
3. 使用`值`解引用指针
4. 支持多级指针，如`指指整`
5. 指针的零值为`空`
6. 结构体指针可直接使用点号访问字段

### 18. 有理数支持
- 有理数类型：`理`
- 分子：`分`
- 分母：`母`

示例：
```go
理数 = 理(2, 3)  // 表示 2/3
分子 = 分(理数)   // 获取分子
分母 = 母(理数)   // 获取分母
```

### 19. 列表推导式
- 推导：`导`
- 范围：`界`

示例：
```go
// 基本列表推导
数段 = [x*x : x <- 1:10]              // 1到10的平方
偶数 = [x : x <- 1:10, x%2 == 0]      // 1到10中的偶数

// 多重推导
矩阵 = [[i+j : j <- 1:3] : i <- 1:3]  // 生成矩阵
```

### 20. 闭包与匿名函数
- 闭包：`闭`
- 匿名函数：直接使用`术`

示例：
```go
术 计数器() 术() 整 {
    计 整 = 0
    还 术() 整 {
        计++
        还 计
    }
}

// 使用闭包
数器 = 计数器()
示(数器())  // 1
示(数器())  // 2
```

### 21. 变参函数
- 变参：`变`

示例：
```go
术 求和(数 ...整) 整 {
    和 整 = 0
    历 数 值 {
        和 += 值
    }
    还 和
}

// 使用变参函数
结果 = 求和(1, 2, 3, 4, 5)
```

### 22. 结构体嵌入
示例：
```go
体 生 {
    名 串
    岁 整
}

体 人 {
    生        // 嵌入生结构
    职 串
}

// 使用嵌入结构
某人 = 人{生: 生{名: "张三", 岁: 30}, 职: "教师"}
示(某人.名)   // 可直接访问嵌入结构的字段
```

### 23. 方法表达式
示例：
```go
体 圆 {
    径 浮
}

术 (圆 圆) 面() 浮 {
    还 3.14159 * 圆.径 * 圆.径
}

// 方法表达式
圆类 = 圆{径: 5}
计算面 = 圆.面
结果 = 计算面(圆类)
```

## 示例代码

### 1. 你好，世界！
```go
术 主() {
    示("你好，世界！")
}
```

### 2. 计算示例
```go
宣 最大数 整 = 100

术 求和(数 整) 整 {
    和 整 = 0        // 局部变量，省略'域'
    计 整 = 1        // 局部变量，省略'域'
    
    循 (计 <= 数) {
        和 = 和 + 计
        计 = 计 + 1
    }
    
    还 和
}

术 主() {
    结果 整 = 求和(最大数)    // 局部变量，省略'域'
    示("求和结果：", 结果)
}
```

### 3. 并发示例
```go
术 主() {
    通 数道 = 创通(整)
    程 函() {
        发 数道 <- 1
    }
    值 := <-收 数道
}
```

### 4. 文件操作示例
```go
术 写文(路 串) 误 {
    文 := 开("测试.txt")
    延 闭(文)
    写 文 "测试内容"
    还 空
}
```

### 5. 类型转换示例
```go
术 转换示例() {
    数 整 = 42
    浮数 = 化(浮64, 数)
    衔值 衔 = 某体
    体值 = 断(衔值, 某体)
}
```

### 6. 集合操作示例
```go
术 集合示例() {
    域 列表 段[串] = 创段()
    增(列表, "测试")
    寻(列表, "测试")
    删(列表, 0)
    长 := 长(列表)
}
```

# 五、未来规划
  完成VSCODE插件开发。
  暂时借用现有GO的编译套件来实现本语言的编译开发过程。
  兼容Go的生态。
