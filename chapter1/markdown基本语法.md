# markdown基本语法

---

### 一、标题

# 这是一级标题
## 这是二级标题
### 这是三级标题
#### 这是四级标题
##### 这是五级标题
###### 这是六级标题

### 二、字体

* 加粗  
**这是加粗的文字**

* 倾斜  
*这是倾斜的文字*`

* 斜体加粗  
***这是斜体加粗的文字***

* 删除线  
~~这是加删除线的文字~~

### 三、引用

>这是引用的内容
>>这是引用的内容
>>>这是引用的内容

### 四、分割线

---
----
***
****

### 五、图片

![样图](/asserts/71155509369_avatar.png)

### 六、超连接

```
[超链接名](超链接地址 "超链接title")
title可加可不加
```
[百度](http://baidu.com "百度一下，你就知道")

### 七、列表

##### 无序列表

* 无序列表
+ 无序列表
  + 子列表
- 无序列表
  - 子列表

##### 有序列表
1. 有序列表
  1. 子列表
2. 有序列表
  3. 子列表
3. 有序列表
  4. 子列表

### 八、表格

语法：
```
表头|表头|表头
---|:--:|---:
内容|内容|内容
内容|内容|内容

第二行分割表头和内容。
- 有一个就行，为了对齐，多加了几个
文字默认居左
-两边加：表示文字居中
-右边加：表示文字居右
注：原生的语法两边都要用 | 包起来。此处省略
```

Issue Id | 6.1.004 | name | component
:-:|:-:|:-:|:-:|:-:
I-07562|B-27127|FOSS ID - introduce http-client-contrib jar to replace source code snippet and remove CMSApplicationTest.java|cms
I-07562|B-27127|FOSS ID - Remove DateParser Snippet from w3c|cms
I-07563|D-09798|FOSSID Remediation: Neptune OAuth Related Code Snippet|neptune
I-07565|D-09801|FOSSID Remediation:EPG Related Code|EPG
I-07560|D-09795|FOSSID Remediation: Contract Related Code Snippet|cms
I-07557|B-27130|FOSSID Remediation: Neptune DigestUtils.java Fixing|neptune
I-07559|D-09792|FOSSID Remediation: Neptune NeptuneRemoteServiceDispatcher.java Fixing|neptune
I-07479|D-09664|Fix the license issue for calendar widget in workflow|workflow
分割线||以下issued 已经在6.1.004之前完成 或 在6.1.004没有相应的defect、backlog|
I-07616|B-27206|FOSSID Remediation: Fix The EPG Checkedbox Widget Issue|EPG
I-07468|D-09623|Fix the ext-js modifications which violate the LGPL License|cms
I-07669|D-09883|FOSSID Remediation: ResettableServletRequestWrapper snippets in contract module|cms

### 九、代码块

* 单行代码  
`echo "这是一行非常牛逼的代码";`

* 代码块  
```
function fun(){
  echo "这是一句非常牛逼的代码";
}
fun();
```

### 十、TODO List

- [ ] task1
  - [ ] task1.1
- [x] task2
  - [x] taks2.1
