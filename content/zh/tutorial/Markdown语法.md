---
title: Markdown语法
date: '2020-03-11T17:22:00+08:00'
toc: false
url: /markdown
draft: false
tags:
  - Markdown语法
---

1. 标题

   ```markdown
   # 一级标题
   ## 二级标题
   ### 三级标题
   #### 四级标题
   ##### 五级标题
   ###### 六级标题
   ```

2. 段落

   段落的换行是使用两个以上空格加上回车，或段落后面使用空行重新开始一个段落

3. 字体

   ```markdown
   *斜体文本*
   _斜体文本_
   **粗体文本**
   __粗体文本__
   ***粗斜体文本***
   ___粗斜体文本___
   ```

4. 分割线

   用三个以上的星号、减号、底线来建立一个分隔线，也可以在星号或是减号中间插入空格。

   > \***
   >
   > \*   \*   \*
   >
   > \-   \-   \-  \-  
   >
   > \------------

5. 删除线

   在文字的两端加上两个波浪线 **~~** 

   ```markdown
   ~~BAIDU.COM~~
   ```

6. 下划线

   通过 HTML 的 \<u>标签来实现

   ```markdown
   <u>带下划线文本</u>
   ```

7. 脚注

   ```markdown
   [^要注明的文本]
   [^要注明的文字]: 要注明解释的内容
   ```

8. 列表

   无序列表使用星号(*****)、加号(**+**)或是减号(**-**)作为列表标记；

   有序列表使用数字并加上 **.** 号来表示；

   列表嵌套只需在子列表中的选项添加四个空格即可。

   ```markdown
   * 第一项
   * 第二项
   * 第三项
   
   + 第一项
   + 第二项
   + 第三项
   
   
   - 第一项
   - 第二项
   - 第三项
   
   1. 第一项
   2. 第二项
   3. 第三项
   
   1. 第一项：
       - 第一项嵌套的第一个元素
       - 第一项嵌套的第二个元素
   2. 第二项：
       - 第二项嵌套的第一个元素
       - 第二项嵌套的第二个元素
   ```

9. 区块

   区块引用是在段落开头使用 **>** 符号 ，然后后面紧跟一个**空格**符号；

   区块是可以嵌套的，一个 **>** 符号是最外层，两个 **>** 符号是第一层嵌套

   ```markdown
   > 区块引用
   > 区块引用2
   
   > 最外层
   > > 第一层嵌套
   > > > 第二层嵌套
   
   列表中使用区块
   * 第一项
       > 区块1
       > 区块2
   * 第二项
   ```

10. 代码

    段落上的一个函数或片段的代码可以用反引号把它包起来（**`**）

    代码区块使用 **4 个空格**或者一个**制表符（Tab 键）**;

    也可以用 **```** 包裹一段代码

    ```markdown
    `printf()` 函数
    ```

11. 链接

    ```
    [链接名称](链接地址)
    
    或者
    
    <链接地址>
    
    链接也可以用变量来代替，文档末尾附带变量地址：
    这个链接用 1 作为网址变量 [Google][1]
    然后在文档的结尾为变量赋值（网址）
    
      [1]: http://www.google.com/
    ```

12. 图片

    ```
    ![alt 属性文本](图片地址)
    
    ![alt 属性文本](图片地址 "可选标题")
    
    这个链接用 1 作为网址变量 [Google][1].
    然后在文档的结尾为变量赋值（网址）
    
    [1]: http://static.google.com/images/google-logo.png
    
    Markdown 还没有办法指定图片的高度与宽度，如果你需要的话，你可以使用普通的 <img> 标签
    <img src="http://static.runoob.com/images/runoob-logo.png" width="50%">
    ```

13. 表格

    - **-:** 设置内容和标题栏居右对齐。
    - **:-** 设置内容和标题栏居左对齐。
    - **:-:** 设置内容和标题栏居中对齐。

    ```
    |  表头   | 表头  |
    |  ----  | ----  |
    | 单元格  | 单元格 |
    | 单元格  | 单元格 |
    
    | 左对齐 | 右对齐 | 居中对齐 |
    | :-----| ----: | :----: |
    | 单元格 | 单元格 | 单元格 |
    | 单元格 | 单元格 | 单元格 |
    ```

14. HTML元素

    ```
    使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑
    ```

15. 公式

    使用两个美元符 $$ 包裹 TeX 或 LaTeX 格式的数学公式来实现

16. 流程图

    * **横向流程图源码格式**

    ```
    ​```mermaid
    graph LR
    A[方形] -->B(圆角)
        B --> C{条件a}
        C -->|a=1| D[结果1]
        C -->|a=2| E[结果2]
        F[横向流程图]
    ​```
    ```

    ```mermaid
    graph LR
    A[方形] -->B(圆角)
        B --> C{条件a}
        C -->|a=1| D[结果1]
        C -->|a=2| E[结果2]
        F[横向流程图]
    ```

    * **竖向流程图源码格式**

      ```
      ​```mermaid
      graph TD
      A[方形] --> B(圆角)
          B --> C{条件a}
          C --> |a=1| D[结果1]
          C --> |a=2| E[结果2]
          F[竖向流程图]
      ​```
      ```

      ```mermaid
      graph TD
      A[方形] --> B(圆角)
          B --> C{条件a}
          C --> |a=1| D[结果1]
          C --> |a=2| E[结果2]
          F[竖向流程图]
      ```

    * **标准流程图源码格式**

      ```
      ​```flow
      st=>start: 开始框
      op=>operation: 处理框
      cond=>condition: 判断框(是或否?)
      sub1=>subroutine: 子流程
      io=>inputoutput: 输入输出框
      e=>end: 结束框
      st->op->cond
      cond(yes)->io->e
      cond(no)->sub1(right)->op
      ​```
      ```

      ```flow
      st=>start: 开始框
      op=>operation: 处理框
      cond=>condition: 判断框(是或否?)
      sub1=>subroutine: 子流程
      io=>inputoutput: 输入输出框
      e=>end: 结束框
      st->op->cond
      cond(yes)->io->e
      cond(no)->sub1(right)->op
      ```

    * **标准流程图源码格式（横向）**

      ```
      ​```flow
      st=>start: 开始框
      op=>operation: 处理框
      cond=>condition: 判断框(是或否?)
      sub1=>subroutine: 子流程
      io=>inputoutput: 输入输出框
      e=>end: 结束框
      st(right)->op(right)->cond
      cond(yes)->io(bottom)->e
      cond(no)->sub1(right)->op
      ​```
      ```

      ```flow
      st=>start: 开始框
      op=>operation: 处理框
      cond=>condition: 判断框(是或否?)
      sub1=>subroutine: 子流程
      io=>inputoutput: 输入输出框
      e=>end: 结束框
      st(right)->op(right)->cond
      cond(yes)->io(bottom)->e
      cond(no)->sub1(right)->op
      ```

    * **UML时序图源码样例**

      ```
      ​```sequence
      对象A->对象B: 对象B你好吗?（请求）
      Note right of 对象B: 对象B的描述
      Note left of 对象A: 对象A的描述(提示)
      对象B-->对象A: 我很好(响应)
      对象A->对象B: 你真的好吗？
      ​```
      ```

      ```sequence
      对象A->对象B: 对象B你好吗?（请求）
      Note right of 对象B: 对象B的描述
      Note left of 对象A: 对象A的描述(提示)
      对象B-->对象A: 我很好(响应)
      对象A->对象B: 你真的好吗？
      ```

    * **UML时序图源码复杂样例**

      ```
      ​```sequence
      Title: 标题：复杂使用
      对象A->对象B: 对象B你好吗?（请求）
      Note right of 对象B: 对象B的描述
      Note left of 对象A: 对象A的描述(提示)
      对象B-->对象A: 我很好(响应)
      对象B->小三: 你好吗
      小三-->>对象A: 对象B找我了
      对象A->对象B: 你真的好吗？
      Note over 小三,对象B: 我们是朋友
      participant C
      Note right of C: 没人陪我玩
      ​```
      ```

      ```sequence
      Title: 标题：复杂使用
      对象A->对象B: 对象B你好吗?（请求）
      Note right of 对象B: 对象B的描述
      Note left of 对象A: 对象A的描述(提示)
      对象B-->对象A: 我很好(响应)
      对象B->小三: 你好吗
      小三-->>对象A: 对象B找我了
      对象A->对象B: 你真的好吗？
      Note over 小三,对象B: 我们是朋友
      participant C
      Note right of C: 没人陪我玩
      ```

    * **UML标准时序图样例**

      ```
      ​```mermaid
      %% 时序图例子,-> 直线，-->虚线，->>实线箭头
        sequenceDiagram
          participant 张三
          participant 李四
          张三->王五: 王五你好吗？
          loop 健康检查
              王五->王五: 与疾病战斗
          end
          Note right of 王五: 合理 食物 <br/>看医生...
          李四-->>张三: 很好!
          王五->李四: 你怎么样?
          李四-->王五: 很好!
      ​```
      ```

      ```mermaid
      %% 时序图例子,-> 直线，-->虚线，->>实线箭头
        sequenceDiagram
          participant 张三
          participant 李四
          张三->王五: 王五你好吗？
          loop 健康检查
              王五->王五: 与疾病战斗
          end
          Note right of 王五: 合理 食物 <br/>看医生...
          李四-->>张三: 很好!
          王五->李四: 你怎么样?
          李四-->王五: 很好!
      ```

    * **甘特图样例**

      ```
      ​```mermaid
      %% 语法示例
              gantt
              dateFormat  YYYY-MM-DD
              title 软件开发甘特图
              section 设计
              需求                      :done,    des1, 2014-01-06,2014-01-08
              原型                      :active,  des2, 2014-01-09, 3d
              UI设计                     :         des3, after des2, 5d
          未来任务                     :         des4, after des3, 5d
              section 开发
              学习准备理解需求                      :crit, done, 2014-01-06,24h
              设计框架                             :crit, done, after des2, 2d
              开发                                 :crit, active, 3d
              未来任务                              :crit, 5d
              耍                                   :2d
              section 测试
              功能测试                              :active, a1, after des3, 3d
              压力测试                               :after a1  , 20h
              测试报告                               : 48h
      ​```
      ```

      ```mermaid
      %% 语法示例
              gantt
              dateFormat  YYYY-MM-DD
              title 软件开发甘特图
              section 设计
              需求                      :done,    des1, 2014-01-06,2014-01-08
              原型                      :active,  des2, 2014-01-09, 3d
              UI设计                     :         des3, after des2, 5d
          未来任务                     :         des4, after des3, 5d
              section 开发
              学习准备理解需求                      :crit, done, 2014-01-06,24h
              设计框架                             :crit, done, after des2, 2d
              开发                                 :crit, active, 3d
              未来任务                              :crit, 5d
              耍                                   :2d
              section 测试
              功能测试                              :active, a1, after des3, 3d
              压力测试                               :after a1  , 20h
              测试报告                               : 48h
      ```

> 节选自[菜鸟教程](https://www.runoob.com/markdown/md-tutorial.html)