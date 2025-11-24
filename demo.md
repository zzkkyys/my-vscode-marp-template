---
marp: true
theme: blue
paginate: true
---

<!-- _class: title -->
# 第一页标题

姓名  |  日期


---

# 1. 标题

```
<!-- _class: title -->
# 第一页标题
```

使用`<!-- _class: title -->`可以为当前幻灯片添加一个自定义的CSS class，这里我们使用了`title`这个class。效果如第一页所示，显示为大标题页。


---
# 2. 脚注

在Marp幻灯片中使用脚注，可以通过Markdown的脚注语法来实现。下面是一个示例：

FN1<sup><a href="#fn1">[1]</a></sup>,  FN2<sup><a href="#fn2">[2]</a></sup>
 
<div class="footnotes">
  <ol>
    <li id="fn1">
      Harbin Institute of Technology, Shenzhen, China
    </li>
    <li id="fn2">
      Guilin University of Electronic Technology, China
    </li>
  </ol>
</div>

---
# 3. 表格

可以在Marp幻灯片中使用Markdown语法创建表格。例如：
| 姓名 | 年龄 | 城市 |
| ---- | ---- | ---- |
| 张三 | 25   | 北京 |
| 李四 | 30   | 上海 |
| 王五 | 28   | 广州 |