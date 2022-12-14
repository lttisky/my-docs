# [markdown基础语法](https://www.cnblogs.com/miki-peng/p/12502985.html)

#### 1. 使用#号标记
```markdown
# 一级标题
## 二级标题
```

#### 2. 字体

```markdown
*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___
```

#### 3. 分隔线:在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格

```markdown
***

* * *

*****

- - -

----------
```

#### 4. 删除线:如果段落上的文字要添加删除线，只需要在文字的两端加上两个波浪线 ~~ 即可，实例如下：

```markdown
~~BAIDU.COM~~
```

#### 5. 下划线:下划线可以通过 HTML 的 <u></u> 标签来实现

```markdown
<u>带下划线文本</u>
```

#### 6. 脚注:脚注是对文本的补充说明，Markdown 脚注的格式如下:

```markdown
[^要注明的文本]
```

#### 7. Markdown 列表
* 有序列表:有序列表使用数字并加上 . 号来表示，如：

```markdown
1. 11111
2. 22222
```

* 无序列表:无序列表使用星号(*)、加号(+)或是减号(-)作为列表标记：

```markdown
* 第一项
* 第二项
* 第三项
------ 分割线 ------
+ 第一项
+ 第二项
+ 第三项
------ 分割线 ------
- 第一项
- 第二项
- 第三项
```

* 列表嵌套: 列表嵌套只需在子列表中的选项添加四个空格即可

```markdown
1. 第一项：
    - 第一项嵌套的第一个元素
    - 第一项嵌套的第二个元素
2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第二个元素
```

#### 8. Markdown 区块

* Markdown 区块引用是在段落开头使用 > 符号 ，然后后面紧跟一个空格符号：

```markdown
> 区块引用
> 菜鸟教程
> 学的不仅是技术更是梦想
```

* 区块中使用列表

```markdown
> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> + 第二项
> + 第三项
```

* 列表中使用区块 :如果要在列表项目内放进区块，那么就需要在 > 前添加四个空格的缩进。

```markdown
* 第一项
    > 菜鸟教程
    > 学的不仅是技术更是梦想
* 第二项
```

#### 9.Markdown 代码

* 单行代码 如果是单行代码或段落上的一个函数或片段的代码可以用反引号把它包起来（`）

```markdown
`printf()` 函数
```

* 代码区块 代码区块使用三个反引号对``` 包裹一段代码，并指定一种语言（也可以不指定）

```markdown
​```python
class CaseData:
    """这是一个存放测试用例数据的类"""
    pass
​```
```

#### 10.Markdown 链接 链接使用方法如下

```markdown
[链接名称](链接地址)

或者

<链接地址>
```

> 高级链接

```markdown
链接也可以用变量来代替，文档末尾附带变量地址：
这个链接用 1 作为网址变量 [Google][1]
这个链接用 runoob 作为网址变量 [Runoob][runoob]
然后在文档的结尾为变量赋值（网址）

  [1]: http://www.google.com/
  [runoob]: http://www.runoob.com/
```

#### 11.Markdown 图片

```markdown
![alt 属性文本](图片地址)

![alt 属性文本](图片地址 "可选标题")

指定图片样式
<img src="http://static.runoob.com/images/runoob-logo.png" width="50%">
```

#### 12.Markdown 表格 :Markdown 制作表格使用 | 来分隔不同的单元格，使用 - 来分隔表头和其他行。

```markdown
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |

-: 设置内容和标题栏居右对齐。
:- 设置内容和标题栏居左对齐。
:-: 设置内容和标题栏居中对齐。

```

#### 13. Markdown 高级技巧
* 支持的 HTML 元素 : 不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写

```markdown
使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑
```

* 转义: Markdown 使用了很多特殊符号来表示特定的意义，如果需要显示特定的符号则需要使用转义字符，Markdown 使用反斜杠转义特殊字符

```
**文本加粗** 
\*\* 正常显示星号 \*\*

Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号
\   反斜线
`   反引号
*   星号
_   下划线
{}  花括号
[]  方括号
()  小括号
#   井字号
+   加号
-   减号
.   英文句点
!   感叹号
```

* [公式](https://www.zybuluo.com/codeep/note/163962#mjx-eqn-eqsample):

```
$$ J_\alpha(x) = \sum_{m=0}^\infty \frac{(-1)^m}{m! \Gamma (m + \alpha + 1)} {\left({ \frac{x}{2} }\right)}^{2m + \alpha} \text {，独立公式示例} $$
```